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

Eclipse Color Theme has issues in it's github repository that represent hints of features to implement and some bugs that have been detected throughout the development process. In addition to this repository, Eclipse Color Theme has a website that allows us to develop new themes to add to the project. 
We saw that we coulnd't delete imported themes one by one, to do that we needed to restore to the default themes and import again all the themes except the one we wanted to delete.

##Identifying components that implement the feature

After analysing the code, we identified the code responsible from saving and showing all the themes that the plugin contains, and the code responsible for saving and reading the thems.

- [ColorThemeManager.java](https://github.com/eclipse-color-theme/eclipse-color-theme/blob/master/com.github.eclipsecolortheme/src/com/github/eclipsecolortheme/ColorThemeManager.java)

In this file we find the implementation of the ColorThemeManager class, where it manages the themes. 

- [ColorThemePreferencePage.java](https://github.com/eclipse-color-theme/eclipse-color-theme/blob/master/com.github.eclipsecolortheme/src/com/github/eclipsecolortheme/preferences/ColorThemePreferencePage.java)

In this file we find the implementation of the preferences page, the one that is show to the user that has the options to apply and import themes.


##Evolution of the feature

When analysing the code, we found that the default themes comes bundled and are saved in the plugin saved preferences and theres isn't direct access to them, but the imported themes are stored in a different place.
The imported themes are read and then the plugin copies all the .xml file converts it to a string and stores.
There isn't a direct way to access or know which one of the themes is the one we want, so we search for each stored theme, extract the .xml converted to string theme, search for the name, and if it is the one, it deletes the theme and removes theme from the themes listing. 

We added a tag to imported themes, to know which theme is imported and which one is default, and a button to delete the theme.

Result below:
![Feature](https://github.com/Miridinia/eclipse-color-theme/blob/master/ESOF-docs/Resources/result.png)


##Pull request

After we developd the feature chosen above, the team submit a [Pull request] (https://github.com/eclipse-color-theme/eclipse-color-theme/pull/256) to the [Eclipse Color Theme Repository] (https://github.com/eclipse-color-theme/eclipse-color-theme) and we are waiting for aprove of the project owner.


![PullRequest](https://github.com/Miridinia/eclipse-color-theme/blob/master/ESOF-docs/Resources/pull.png)


##Conclusion

//TODO

##Contribuition of the team members

we feel that the variation between different people and their work doesn't warrant an unalike division of the contribution, therefore, we also apply 25% to each individual member of the team.
