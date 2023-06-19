The project creator is the most important tool on the homepage. It provides the necessary tools for dynamically creating projects. Manual creation of customized projects can be tedious and time-consuming, so a script was developed to automate the project creation process. Himawari2D projects are essentially Java Maven projects with various Java files that make up the engine, as illustrated in Chapter 6. However, these files are relative and need to be modified depending on various factors. The main purpose of the project creator is to simplify the process of factoring these files and provide other utilities such as the creation of useful objects and templates.

Below is an illustration of the project creation interface. It has a "Create Project" button that triggers the previously described process, an "Open Project" button that opens one of the recent projects, which are stored in a file to remember the programmer's history. Projects can be selected from the dropdown box displayed below. If no project is selected, a folder selection dialog opens to choose a project location on the computer.

![Pasted image 20230608193554.png](images/Pasted%20image%20230608193554.png)

Below the basic project control buttons, there are advanced project creation menus. The project creation settings menu consists of six checkboxes:

1. Add Main Object: Creates an initial empty object within the project.
2. Add Configured Camera Object: Adds a 2D camera object that is ready to follow an object.
3. Use Gson Library: Gson is a library that allows reading, writing, and processing JSON files.
4. Use Jackson Library: Jackson is a library that enables processing of various file types, including XML.
5. Use SLF4J Library: SLF4J is a simple logging library for Java, widely used for creating references to the game's output and identifying runtime issues.
6. Use JBullet Library: JBullet is a powerful library supported by various languages that enables realistic physics simulation. While Himawari2D supports physics simulation as mentioned in Chapter 6.5, it may be too basic for certain projects.

The other menu shown below is the template selection menu. These templates have been developed to provide programmers with a ready-to-use game base. The templates also include example projects for learning the framework, which will be explained in more detail in a future chapter.

The project templates are illustrated below:

![Pasted image 20230608193625.png](images/Pasted%20image%2020230608193625.png)