# Java Hello World experience from Ernie Van Duyne


I took the Java basic course at Team Treehouse - 
https://teamtreehouse.com/library/java-basics
-----------
## Set Up
In order to run Java I decided to install the Eclipse IDE.
         
         - http://www.eclipse.org/getting_started/

### Observation
I saw that there was different version of the IDE:
Java SE = Standard Edition. This is the core Java programming platform. It contains all of the libraries and APIs that any Java programmer should learn (java.lang, java.io, java.math, java.net, java.util, etc...).
Java EE = Enterprise Edition. From Wikipedia:
The Java platform (Enterprise Edition) differs from the Java Standard Edition Platform (Java SE) in that it adds libraries which provide functionality to deploy fault-tolerant, distributed, multi-tier Java software, based largely on modular components running on an application server.
In other words, if your application demands a very large scale, distributed system, then you should consider using Java EE. Built on top of Java SE, it provides libraries for database access (JDBC, JPA), remote method invocation (RMI), messaging (JMS), web services, XML processing, and defines standard APIs for Enterprise JavaBeans, servlets, portlets, Java Server Pages, etc...
If you are new to Java, definitely start with Java SE.
---------------
After I installed Eclipse it offers both a hello world tutorial and other starter Java tutorials.

I took the step by step Eclipse Hello World Tutorial and came up with this - 

`public class HelloWorld {
	public static void main(String[] args) {
System.out.println("Hello world!");
	}
}`
 
Setting up the Eclipse environment had a couple of small hiccups but it was fairly easy.
Eclipse automatically compiled and ran the class  - all I had to do was click on a run icon.

I next continued the course on Team Treehouse to see if they had a different approach and in fact they did!

I created a class which used Console instead of System in the Eclipse tutorial.
I needed to import the Console class in order to use it also.

`import java.io.Console;
 public class Introductions {
    public static void main(String[] args) {
        Console console = System.console();
      console.printf("Hello World");       
  }
}`


I next had to compile it:

_treehouse:~/workspace$ javac Introductions.java_                                                                                                                   
_treehouse:~/workspace$ ls_                                                                             
_Introductions.class  Introductions.java_


I then ran it using the following: 
                                                              
*treehouse:~/workspace$ java Introductions*                                                            
*Picked up JAVA_TOOL_OPTIONS: -Xmx128m*                                                          
*Picked up _JAVA_OPTIONS: -Xmx128m*

And the output was:

	*Hello World*


###Observation
I attempted to use console.printf("Hello World"); in the Eclipse IDE but I got a null pointer error.
Upon investigation I discovered the following - 

 You are using eclipse tool or may be another tool to run this program , because eclipse runs your program as a background process and not as a top-level process with System console or depend on d IDE handling of console io.


 In IntelliJ IDEA there is the same problem. The issue is that most IDEs to run programs use program javaw instead of java. This program runs without any link with system console but it supports input/output streams. IDEs use their own way to communicate and input information during program flow it uses System.in, System.out to show all needed information in prepared tab called probably "Console" (I don't use Eclipse ;))

