# Setting up a new Gradle Project

## Table of Contents
- [Overview](#overview)
- [Step-by-Step Guide](#step-by-step-guide)
- [Common Challenges](#common-challenges)
- [Further Studies](#further-studies)

## Overview
This guide illustrates how to set up a Gradle project from scratch without any hassle.

Assuming you already know what Gradle is, you can skip the remainder of this section and move on to the next.

In simple terms, Gradle is a build tool used to automate the building, testing, and deployment of software projects. It has become popular in recent times compared to its counterpart, Maven, due to its performance advantages and its design for modern frameworks.

---
## Step-by-Step-Guide
+ Ensure that you have gradle installed, you can easily verify this by entering the following command
  ```
  gradle v
  ```
  This should return the version of Gradle you have installed. However, if you receive an error, you can follow the instructions on how to install Gradle here:
  [Installing gradle](https://docs.gradle.org/current/userguide/installation.html)

+ Create a new directory. You can either do this manually or via the command line with
    ```
    mkdir my_new_gradle_project
    ```
+ Navigate to the directory with the following command
     ```
    cd my_new_gradle_project
    ```
+ Initialise the gradle project as this would help set up the build files
  ```
  gradle init
    ```
  During this process, you will need to answer a few questions, usually pertaining to the type of project and the build script DSL
  ![Gradle_BuildType](./Gradle_buildType.jpg)
  **I recommend selecting "basic" as the build type, as it serves as a solid foundation for further development.**

  ![Gradle_BuildScript](./GradleBuildScript.jpg)
  **Your choice here mainly depends on what domain specific language you are familiar with.** 

+ After that is done you should now have an initial set up that should look like this:
  ![Gradle_Setup](./Gradle_Project_after_init.jpg)
  A variety of Gradle files will be generated; however, the most important ones are build.gradle.kts, settings.gradle.kts, the .gradle directory, and the Gradle wrapper. The build.gradle file is the main build configuration file for the project, where most of the build settings will reside. The settings.gradle file contains settings that Gradle reads before starting your build (for instance, the root project name). The Gradle wrapper ensures everyone working with the project is using the same version of Gradle.
  
---
## Common Challenges
In this section, we would highlight some common challenges that may be associated with setting the gradle project
as described above:
+ The gradle -v command returns an error even when Gradle is installed. In that case, ensure that it has been added to the system's PATH correctly.
+ Unfamiliarity with the command line. If you are not comfortable with command line usage, please refer to
  [Command line basics](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Understanding_client-side_tools/Command_line).
+ The number of generated files may be overwhelming, especially for newcomers. Knowing which files are crucial and their purposes is essential.

---
## Further Studies
For further studies on Gradle and general questions about using Gradle, please refer to the
[Gradle documentation](https://docs.gradle.org/current/userguide/gradle_basics.html)
