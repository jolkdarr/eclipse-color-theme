#NOTA > https://github.com/eclipse-color-theme/eclipse-color-theme/issues/108




#Verification and Validation
![Eclipse-Color-Theme](http://p2.pdt-extensions.org/images/colorthemes/screenshot.png)
Team and contact:
* Carolina Moreira - up201303494@fe.up.pt
* Nuno Silva - up201404380@fe.up.pt
* Paulo Babo - up201404022@fe.up.pt
* Rita Carvalho - up201304918@fe.up.pt

##Introduction

The goal of this report is to analyze the processes of verification and validation (V&V) followed in the development of Eclipse Color Theme, with the description of some features of this project witch concern the applicationof these processes.
First of all, we explore the degree of software testability, analysing the controllability of states of the components tested, the observability of the results and the insulation of the components, as well as the degree of separation of functionalities, the intelligibility of the components and the heterogeneity of the technologies used.
In a second step, we present some relevant statistics related with the verification and validation of software in the Eclipse Color Theme.
Finally, will be presentes the results of the exercise, realized by the authors of this report, that consist in the selection of a bug report from the list of issues of the project, the design of test cases for it's reproduction and the effective correction of the error.

##Software Testability

Concerning testability, Eclipse Color Theme seems to be weel struture. The arquitecture of the plugin, based packages, introduces a modularity that makes it simple and efficient to separete the tests to run, while it's base, the Eclipse Color Theme package, allows the cohesion and communication between the diferrent components, so you can also test communication aspects in different modules easily.
In the following subsections will be analyzed in more detail the various aspects that allow to evaluate the characteristics of testability.

###Controllability

Eclipse Color Theme features a code organization and object-oriented programming paradigm, drawing on the capabilities that java confers in this area. The programming language used provides the appropriate tools to allow the complete and controlled manipulation of both the behavior of the instantiated objects and the value of the data stored in them. The unit tests tend to be oriented to the study of the behavior of the packages, and it's context is abstracted using several techniques, which will be discussed in greater depth in the section on Isolability It is therefore possible to understand that the controllability characteristics of the Eclipse Color Theme components fit particularly well for performing unit tests.

###Observability

The Eclipse Color Theme tests are run in Eclipse according to the tests project of the plugin .
The distributed nature of open-source projects seems to require that not only the observability of the test results on the changes made by each programmer be guaranteed, but also that it's possible to analyze the results of the tests run on code developed by third parties and is not yet integrated into the project code base. However it is something that this project still does not dominate totally being that the tests are mainly realized by the project owners.

###Isolability




Discuss Software Testability and Reviews: controllability, observability, isolateability, separation of concerns, understandability, heterogeneity.  
Grade: 6pts
Report Test Statistics and analytics:  e.g., number of test cases, percentage of coverage, number of flaky tests, etc. (see links of projects in moodle for inspiration)
Grade: 8pts
Identify a new bug and/or correct a bug
Grade: 6pts (identification: 4 points; correction: 2 points)
You think your project has no bugs?! Then, you do need to have a compelling story for us to credit you 6pts! 
