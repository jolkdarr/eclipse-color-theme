#Software Design
![Eclipse-Color-Theme](http://p2.pdt-extensions.org/images/colorthemes/screenshot.png)
Team and contact:
* Carolina Moreira - up201303494@fe.up.pt
* Nuno Silva - up201404380@fe.up.pt
* Paulo Babo - up201404022@fe.up.pt
* Rita Carvalho - up201304918@fe.up.pt

##Introduction

This report aims to explain the Eclipse Color Theme architecture according to 4 + 1 view model of software architecture.
We begin to make an approach to  4 + 1 view model of software architecture and in the next points we approach a little more specific in respect to Logical view, Development view, Deployment view and Process view, with the help of illustrative diagrams.

##4+1 Architectural View Model

The 4+1 Architectural View Model was designed to describe the architecture of the software-intensive systems based on the use of multiple views. This views are used to describe the system from the viewpoint of different stakeholders. The four views of the model are logical, development, process and deployment view. The "plus one" view are the use cases that were approached in the second report.

The logical view is concerned with the functionality that the system provides to end-users, and is represented with class diagram, activity diagram and state diagram. 

The development, represented with the package diagram, view illustrate the system from a programmer's perspective and is concerned with the software manegement. 

The process view, illustrated with the activity diagram, deals with the dynamic aspects of the system, explains the system processes and how they communicate, and focuses on the runtime behavior of the system. 

At last, the deployment view despicts the system from a system engineer's point of view. It's concerned with the topology of the software components on the physical layer, as well as the physical connections between these components. This view is represented with the deployment diagram.


##Logical View (Nuno)

TODO, diagrama e falar sobre os packages

##Development View (Carolina)

##Deployment View (Paulo)

##Process View (Rita)

//TODO, diagramas

In this topic we consider the Eclipse as the system because the Eclipse Color theme is just a pluggin and the approach of this view to the plugin is quite simple. 
As we said before, this view show the different processes of the system as well as their interactions in run-time. The Eclipse text editor allows the execution of a quite diverse set of activities, being necessary to implement a very diverse set of features that operate directly or indirectly on the text buffer to edit. In this report, we opted to illustrate the basic handling of text buffers and clipboards, and the operations that allows to save and open text files and buffers.

The diagram below represents the operations that allows to save and open text files and buffers. 

![LoadAndSaveFile](https://github.com/Miridinia/eclipse-color-theme/blob/master/ESOF-docs/Resources/Load%20and%20Save%20file.jpg)


##Contribuition of the team members




Introduction to Software Architecture and the 4+1 Architectural View Model; What are the architectural patterns followed by your project (if it doesn't follow any well known one, discuss whether it would be best to do so).
Grade: 4pts

Logical View
Grade: 4pts

Development View
Grade: 4pts

Deployment View
Grade: 4 pts

Process View
Grade: 4 pts
