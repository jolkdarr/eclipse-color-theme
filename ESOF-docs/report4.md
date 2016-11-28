#NOTA > https://github.com/eclipse-color-theme/eclipse-color-theme/issues/108
Não conseguimos replicar o bug, funcionava direito, pedi mais informação e estou à espera de resposta.



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
Finally, will be presentes the results of the exercise, realized by the authors of this report, that consist in the selection of a bug report from the list of issues of the project, the design of test cases for it's reproduction and the attempt of correction of the error.

##Software Testability

Concerning testability, Eclipse Color Theme seems to be weel struture. The arquitecture of the plugin, based packages, introduces a modularity that makes it simple and efficient to separete the tests to run, while it's base, the Eclipse Color Theme package, allows the cohesion and communication between the diferrent components, so you can also test communication aspects in different modules easily.
In the following subsections will be analyzed in more detail the various aspects that allow to evaluate the characteristics of testability.

###Controllability

Eclipse Color Theme features a code organization and object-oriented programming paradigm, drawing on the capabilities that java confers in this area. The programming language used provides the appropriate tools to allow the complete and controlled manipulation of both the behavior of the instantiated objects and the value of the data stored in them. The unit tests tend to be oriented to the study of the behavior of the packages, and it's context is abstracted using several techniques, which will be discussed in greater depth in the section on Isolability It is therefore possible to understand that the controllability characteristics of the Eclipse Color Theme components fit particularly well for performing unit tests.

###Observability

The Eclipse Color Theme tests are run in Eclipse according to the tests project of the plugin .
The distributed nature of open-source projects seems to require that not only the observability of the test results on the changes made by each programmer be guaranteed, but also that it's possible to analyze the results of the tests run on code developed by third parties and is not yet integrated into the project code base. However it is something that this project still does not dominate totally being that the tests are mainly realized by the project owners.

###Isolability

The Isolability of the different components of Eclipse Color Theme is evident. Each component works by itself, there being separation between themes and mapping editors. So your individual testability in terms of unit testing is effective because it can be considered that the project is below a black box model where external changes (including changes to input level) don't influence the test results.
To enable testing the plugin, another test project is being used where unit tests are being developed and that allows the developer to test his code in a completely isolated way.

###Separation of responsibilities from each component

In the context of validation and verification of software requirements a strict separation of components is highly advantageous from the point of view of the ease of definition of the test definition that is exhaustive as to the behavior of each functionality, testing it not only correctly but also integrally. A feature that takes on too many responsibilities or responsibilities from very different forums is not only more susceptible to the introduction of crashes when changed, but also more difficult to test and validate.
The Eclipse Color Theme architecture is, as already mentioned, package based, which are responsible for implementing various components in the context of the fully functional plugin. Thus Eclipse Color Theme presents an external structure of highly segmented and clearly defined responsibilities, reserving for itself only the role of coordinator of the various core packages to the correct functioning of the plugin.
Analyzing the internal structure of Eclipse Color Theme, it is observed that it explicitly separates its functionality by several packages. The separation of responsibilities is ensured quite strictly, where the themes are isolated from the mapping editors.

###Understanding

Despite it's open-source nature, which would imply that the documentation was explicit and concise so that it could be quickly consulted and apprehended by as many people as possible, Eclipse Color Theme isn't well documented. The information obtained is confusing and it is difficult to get in touch with the project owners for more information.
The architecture of Eclipse Color Theme is quite simple, resulting in it's careful separation of responsibilities into a set of packages whose names and behaviors work well for a person to understand the terminology to which the package refers. Having said this, the lack of documentation is outweighed by the ease in understanding the code, allowed to be studied by an adequate understanding of each component.

###Heterogeneity

In the Eclipse Color Theme repository another test project is available. These tests are mostly unit tests.
Eclipse Color Theme is a very heterogeneous plugin from a technological point of view, which is clearly reflected in your suite of tests. The definition of specifications is done in Java.

##Test Statistics and analytics

As already mentioned, Eclipse Color Theme provides another test project in it's repository where unit tests are performed. At present there seem to be 6 different unit tests and the tests so far developed are:

* ColorTest
* ColorThemeMappingTest
* ColorThemeSemanticHighlightingMappingTest
* ColorThemeSettingTest
* ColorThemeTest
* MockEclipsePreferences

It should also be noted that these tests are performed in Java.

##Bugs

Eclipse Color Theme has a list of issues that reveal project bugs as well as new ideas to develop. In fact, in the documentation they advise to open a new issue, if we have a new idea, or if we want to contribute and we have no idea, to see the issues that are still open and start working.
Currently, Eclipse Color Theme has 105 issues open and 77 issues closed. Of these open issues, what seems most appealing is the issue [Bracket color ignored] (https://github.com/eclipse-color-theme/eclipse-color-theme/issues/108).
This issue depicts a bug where the color bracket is ignored, and it is this bug that we intend to correct. However we couldn't replicate the bug once it worked right. So we try to get in touch with the developers asking for more information and we are still waiting for an answer.

##Conclusion

//TODO

##Contribuition of the team members

Although the work was more distributed than in the previous report, we feel that the variation between different people and their work doesn't warrant an unalike division of the contribution, therefore, we also apply 25% to each individual member of the team.
