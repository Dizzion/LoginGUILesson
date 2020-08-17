![Java Logo](https://www.clipartkey.com/mpngs/m/107-1073107_java-programming-language-logo.png)
# Making a Login window through Java

We are going to make a Login GUI using the Java programing language. Since we have gone over a little bit with the Bagel Shop GUI and how it looks when we have a file system in Java we are going to code a Login GUI that will run on a basic window that we could make an executable that runs on websites or desktop applications.

***
## **_3-5min_**
In order for Everyone to get started and code along, if they want, we need to download the Java language Support for VScode here -> [Java](https://code.visualstudio.com/docs/languages/java).
There is an install for both windows and macOS on that page for linix users you will need to download the JDK I suggest just following along but here -> [JDK](https://www.oracle.com/java/technologies/javase-downloads.html) is the JDK standalone installer. This second step also follows for those that use other IDE's. For those looking for an IDE just for Java [Eclipse is the best out there.](https://www.eclipse.org/downloads/packages/)

### Once this is done go ahead and clone or (fork and clone) this repo, so we can code it together.

---
## _~25min_

## **_In this lesson we will:_**
* Import Events to so that we can make a gui from basic components
* Set components to certain sections of the GUI with layout
* Learn Action Listeners in Java
* Learn to Check basic Login information using Java
* Talk about Databases in Java and the routes associated with them

***
# **_Importing java dependencies_**
We are going to look at two java dependencies and what they are doing for us and getting back for us to use in our program.

## JPanel
JPanel comes from the dependency ```javax.swing.*``` when using this syntax we are getting all parts of JPanel rather than having to call them all individually. If we were going to call them all individually we would need to do:
```Java
import javax.swing.JPanel;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JTextField;
import javax.swing.JButton;
import javax.swing.JPasswordField;
```

## Action Listeners in Java
Yes we need to import these from the Java dependencies too. I know seem like how will I remember this when I would need to use this wile coding it at a later time..... Well first I'll say practice make perfect the more you do something the more likely you are going to remember with dependencies you will need. But refering to your old projects is always a good source of googling the dependencies you need works just as well.

Anyway.... Lets get back to Action Listener dependencies. For this one we will nee ```java.awt.event.*``` as we get deeper into dependencies it is going to want you to get more specific with your calls but you can still grab good sized dependencies without memory yelling at you.

***

# **_Set Components and declare our class_**
We are going to start by declaring our base class implementing our action listener and declaring our global variable.

## Classes through Java
When we are declaring our class in Java documents they are our code blocks beginning and end point besides importing our roles from java everything that runs in the program lives within a class.

Our base class with alway look something like this:
```Java
public class GUI implements ActionListener 
{
    // Code Here
}
```
Now you will notice unlike javascript we are not leaving our curls on the end that is just syntax for most large memory based programs so that you have a cleaner collapse with collapsing code to get a bigger view.

---
## Global Variables
In javascript we would just declare these at the top of the file but in Java they need to live inside the class so that they can be used in it or accessed from outside the class through it.

### Private Variables
Private variables are hidden from reference and can not be accessed by outside sources as opposed to public.

### Public Variables and Functions
Public functions and variables can be acessed from outside the class it is declared in. So if I wanted to access it from another file and layer components through different files and classes I could do that in public form.

***

# **_Making our main function_**
Now we are going to start writing the function that runs our program.

## Main
The main function is not a syntax case and needs to be declared as ```public static void main(String[] args)``` by calling this function as void we do not have to return a value at the end of the function. Inside the parentheses we are using ```String[] arg``` as our arguments for the code debugger and runner. So that java knows which function to run our program from and other classes to interact with.

## Other Functions inside a class
The main function is just that a function you can declare and write out other functions for the program to use any where **WITHIN** the class it was called. The only time you can call a function from another class in another file is when that file is within the same directory as the parent java file (aka the main function program)

***

# **_Setting Variables and properties_**
Setting variables and declaring them is a bit different in Java than Javascript we need to make sure we choose what type that variable will be when we declare it. Note you can **NOT** change it later. So if I need a variable that holds a basic number that doesn't get to large I would use ```int number;```. Notice I don't delcare what the value of that variable is this is because we don't have to declare values when a variable is make in most memeory based languages.

## Variables for out GUI
When we are setting the Panel and Frame variables for our program we are taking those classes from the Java library to we need to delcare them as a JPanel variable that is a new JPanel().

## Setting properties of Declared Class Variables
We can change the properties of a class that call into a variable by just calling the function that is inherited from the parent so frame.setSize will allow us to set the size of our frame to what we want it.

***

# Q/A
Ask questions you can never ask too many questions when looking at a new language.
