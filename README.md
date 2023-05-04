Download Link: https://assignmentchef.com/product/solved-cs9053-assignment-1
<br>



This assignment will give you some practice on the basics of what you’ll be doing in your more complex Java Assignments – setting up a program, printing output, receiving input/arguments, and doing basic calculations.

<strong>Part 0 (Ungraded)</strong>

<ol>

 <li>This is to get you started. I will be using the Eclipse IDE available at <a href="https://eclipse.org">http://eclipse.org</a>.</li>

</ol>

The IDE (Integrated Development Environment) is the application where you will be writing and executing your code. However, the compiler is separate. Eclipse does have its own built-in compiler for PC and Linux users, but MacOS users will have to install the Java Development Kit (JDK) on their own.




I highly suggest all of you install the JDK on your own. We will be using Java 1.8, but all JDK versions about 1.8 will be able to compile for that version. Use whatever method for downloading and installing your JDK is and. Put the bin directory for the JDK in your PATH. Type “java -version” in your terminal and you should get a result like this, depending on your exact version:




java version “1.8.0_45”

Java(TM) SE Runtime Environment (build 1.8.0_45-b14)

Java HotSpot(TM) 64-Bit Server VM (build 25.45-b02, mixed mode)




Then in Eclipse under the Eclipse menu go to Preferences … Java … Installed JREs




After installing your JDK you will want to click on “Add” and specify the directory where your JDK is.




<ol start="2">

 <li>Now that you have Eclipse working and have your workspace set up, you’ll want to get started with the Assignment 1 Code.</li>

</ol>




Download Assignment1.zip from the NYU Classes page. There are a couple ways of importing the project into your workspace, but the easiest is to unzip Assignment1.zip into your workspace, and then Click on File … Open Projects from File System and click on the directory Assignment1




<ol start="3">

 <li>In the Part0 folder, open the default package, and then the HelloWorld.java file. In the file, right click on Run As … Java Application. In the console, beneath the code, it should print “Hello, World!”</li>

</ol>




<ol start="4">

 <li>In the HelloWorld.java code window, move your mouse just to the left of the number six, which indicates the line number. Double click on it, and a blue dot should appear.</li>

</ol>




This is a breakpoint. It will stop the code when you’re running in debug mode. Right click in the code window and click on Debug As … Java Application. You will see something like this:

The code has stopped at line 6, and nothing has printed out on the console (yet). From here, there are two things you can do. If you look at the right side of the toolbar, you will see a “Play”, “Stop”, “Step into” and “Step over” controls:

If you press the “play” button, the program will complete.  If you press the “stop” button, the program will end. If you press the “Step over” button (second arrow button after the “Stop” button), the program will print out “Hello World!” and proceed to line 7. Press it again and the program will complete.




<ol start="5">

 <li>Let’s take a look at what’s going on “under the hood.” In your terminal window go to your Assignment1</li>

</ol>



















Look in the directory Part0 and your HelloWorld.java code should be there. Then look in the bin directory. There should be a program called HelloWorld.class. From the bin directory, type java HelloWorld. This should output “Hello World!”.




Now, delete HelloWorld.class and go back into the Assignment1 directory. Execute the Java compiler with javac -d bin/ Part0/HelloWorld.java. In the bin directory you should see the HelloWorld.class file while you just created. This is the compiled Java bytecode program you’ve just created, and you can run it with java HelloWorld and get the same result. Obviously, Eclipse does all of this for you, but you should see how it works yourself.




(Most problems will not be 3 ½ pages long. This is just something to get you started)







<strong>Part I – Printing Output</strong>




<ol>

 <li>Print out your initials using “big letters”. Everyone calls me “Dean”, and my middle name, the spelling of which is beyond the scope of this assignment, starts with a K, so I would print out DKC like so:</li>

</ol>




DDDD   K   K   CCC

D   D  K  K   C   C

D   D  K K    C

D   D  KK     C

D   D  K K    C

D   D  K  K   C   C

DDDD   K   K   CCC




Using the MyInitials.java class, do the same for your initials using System.out.println statements. Here’s a guide to big letters:




<ol start="2">

 <li>In the file java, there are a set of statements that execute mathematical operations. Using System.out.println() statements, print out the results of these operations that is assigned to the variables. They should have the format:</li>

</ol>




the value of a is [Value]




You can step through each of these statements using breakpoints and the debugger if you want, to see out it works, and you can see the variable values in the “expressions” tab to the right of your code window.







<strong>Part II – Input</strong>

<strong> </strong>

<ol>

 <li>Look at the file java. What this does is prompt you to enter your name, and it assigns what the user types to the variable “name.”</li>

</ol>




Have the program take the variable “name” and use it to print out:




Hello, [name]!




Where [name] is the value of the variable “name”.




<ol start="2">

 <li>This will show you how to pass command-line arguments into your main method and use those in your program. First, open the file java</li>

</ol>




Next, go to Run … Run Configurations. It will open this window:




You are going to create a “GetNameArgument” run configuration and associate it with the class GetNameArgument.




Then click on the “Arguments” tab and set the command line argument and set your name as the command line argument




We are only using one command line argument, but command line arguments are separated by spaces. The first command line argument can be accessed with args[0].




Write a program that prints out “Hello [name]!” using the command line argument in args[0].


