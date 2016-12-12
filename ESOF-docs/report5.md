Feature: ???
How did you locate the parts in the source code that needed to be modified ????

#Software Maintenance/Evolution
![Eclipse-Color-Theme](http://p2.pdt-extensions.org/images/colorthemes/screenshot.png)
Team and contact:
* Carolina Moreira - up201303494@fe.up.pt
* Nuno Silva - up201404380@fe.up.pt
* Paulo Babo - up201404022@fe.up.pt
* Rita Carvalho - up201304918@fe.up.pt

##Introduction

This report aims to discuss the Software Maintainability according SIG metrics and to describe the development of a new feature, exposing it's development process from it's identification, the identification of the components that implement the feature, and the submission by a pull request of the feature.

##Software Maintainability

According the report [Better Code Hub](https://github.com/Miridinia/eclipse-color-theme/blob/master/ESOF-docs/Resources/Better%20Code%20Hub.pdf) the compliance of the project Eclipse Color Theme is 6 in 10. The project failed in the next metrics:

* Write Short Units of Code
* Write Code Once
* Keep Architecture Components Balanced
* Automate Tests

Writing small units of code makes it easy to understand, reuse and make code easy to test. According to the report, when writing new units, we don't should let them grow above 15 lines of code and, when it grows, we should slitting them into smaller units. This project failes in this metric because we have one block with more than 60 lines of code, 4 blocks with more than 30 lines of code which difficult the understanding of code and the test of it. This metric explain the difficulty by our team in understandind the project.

The project failes in the metric Write Code Once because we have multiple duplicated blocks of code and this duplication forces the bugs to be fixed in multiples places and this is inefficient and error prone.

Keep the Architecture Componentes Balance begin to balancing the number and relative size of the components to make easier to locate code. In this project we have only one component where we should be between 2 and 12, so we can't compare the size of the components. A way to improve this balanced is organising the components based on functionality and divide the project code into components.

Once this project is a small system we should have at least some test code and one assertion to make the development more predictable and less risky. Once the Eclipse Color Theme is a open source project that uses github, a simple way to improve the metric of Automate Tests is to synchronized the repository of this project from Github with [Travis CI] (https://travis-ci.org).

##Identification of a feature

Eclipse Color Theme has issues in it's github repository that represent hints of features to implement and some bugs that have been detected throughout the development process. In addition to this repository, Eclipse Color Theme has a website that allows us to develop new themes to add to the project. And with the help of the 'Better Code Hub' we can see where this project should be improved.
Saying this, the feature we decided to implement was //TODO because it's acessible in terms of complexity and given the time available, this feature is the most opportune.

##Identifying components that implement the feature

//TODO

##Pull request

After we developd the feature chosen above, the team submit a pull request to the [Eclipse Color Theme Repository] (https://github.com/eclipse-color-theme/eclipse-color-theme) and we are waiting for aprove of the project owner.

//INCLUIR IMAGEM E LINK DO PULL REQUEST

![PullRequest](https://github.com/Miridinia/eclipse-color-theme/blob/master/ESOF-docs/Resources/pull.png)

https://github.com/eclipse-color-theme/eclipse-color-theme/pull/256

##Conclusion

//TODO

##Contribuition of the team members

we feel that the variation between different people and their work doesn't warrant an unalike division of the contribution, therefore, we also apply 25% to each individual member of the team.
