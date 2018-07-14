# DebugWindow
A small utility in Java to help manage debug and exception handling on GUI projects


# What is this?
While working with Java GUI I have always struggled to debug due to the different behaviour that the environment can have between my development environment (Netbeans, usually) and the same application launched from a JAR.
To aid me in the development of GUI application that will be launched from a JAR,  I created this small utility that can be packed with the main application and that will take care of handling exception and eventual debug mesages.

# How does it work?
It's a pretty simple utility. Only one window, developer with Netbeans included GUI editor, and a singleton class to invoke it.
After being initiated with the factory method, it will automatically capture every exception not handled and every print on both stdout and stderr.
This informations will be available on a custom frame where the list of exception, with full stacktrace, and the two streams can be read as needed.