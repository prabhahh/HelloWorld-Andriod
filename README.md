Experiment 1: Develop a Simple “Hello World” Android Application
1. Experiment Details
Experiment Number: 1
Experiment Title: Develop a Simple “Hello World” Android Application
Platform: Android
Development Environment: Android Studio
Programming Language: Kotlin or Java, depending on the project configuration
Application Output: Hello Android!
2. Aim
To develop, build, and run a basic Android application that displays a greeting message, “Hello Android!”, on the mobile screen.
3. Objectives
The objectives of this experiment are:
To understand the basic process of creating an Android application.
To become familiar with the Android Studio development environment.
To understand the purpose of an Activity in an Android application.
To learn how text can be displayed on an Android screen.
To build and run an application on an Android emulator or physical device.
To observe the application's output and capture a screenshot.
To document the application and its test cases for a GitHub submission.
4. Software and Hardware Requirements
Software Requirements
Android Studio
Android SDK and the required build tools
Kotlin or Java, according to the project configuration
Gradle build system
Android Emulator, or USB/Wireless debugging for a physical Android phone
Git and a GitHub account for version control and submission
Hardware Requirements
A computer capable of running Android Studio
An Android emulator or Android smartphone for running the application
A USB cable if a physical phone is connected by USB
5. Concept and Technology Behind the Experiment
Android applications are commonly developed using Android Studio. A typical Android project contains source code, resources, a manifest file, and build configuration files. These parts work together to build and launch the app.
5.1 Android Studio
Android Studio is the official integrated development environment (IDE) for Android app development. It provides tools to write code, design interfaces, build projects, find errors, and run applications on emulators or physical devices.
5.2 Activity
An Activity represents a screen in an Android application. It controls a screen's behaviour and can display the user interface. In a simple starter project, MainActivity is often the first screen shown when the app launches.
5.3 User Interface (UI)
The user interface is the part of the application that the user sees and interacts with. In this experiment, the UI is intentionally simple: it displays the text “Hello Android!” against a dark background.
Depending on the Android Studio template, the screen can be created using XML layout resources, Jetpack Compose, or UI elements created in source code. The exact implementation may differ between projects.
5.4 AndroidManifest.xml
The manifest file describes important information about the application to the Android system. Depending on the project, it identifies the application's components and declares which Activity can be launched.
5.5 Gradle
Gradle is the build system used by Android projects. It helps compile the source code, process resources, and package the application so that it can be installed and run.
5.6 Output Screenshot
A screenshot provides visual evidence that the application has launched and displays the intended message. The screenshot included in this repository shows “Hello Android!” on the device screen.
6. Scenario Used to Demonstrate the Experiment
A student is developing their first Android application and wants to verify that the development environment is working correctly. The student creates a simple app that displays a greeting when opened.
When the application launches, the text “Hello Android!” appears on the screen. This small example demonstrates the basic development workflow: create a project, configure it, build it, run it on a device, and check the output.
7. Procedure
Open Android Studio on the computer.
Select the option to create a new Android project.
Choose a basic Activity template suitable for the course.
Enter the project name, package name, programming language, and minimum SDK required by the project.
Allow Android Studio to create and sync the project.
Open the main Activity or the screen layout used by the project.
Add or retain a text component that displays “Hello Android!”.
Check that the text is readable and visible on the screen.
Connect an Android phone or start an Android emulator.
Build and run the application.
Confirm that the app launches and the greeting appears.
Capture the output screenshot.
Add the source code, README, and screenshots to the GitHub repository.
8. Source Code Overview
The exact source code depends on the template selected in Android Studio. In a traditional Activity-based project, MainActivity.kt or MainActivity.java contains the screen logic, and an XML layout may define the text component. In a Jetpack Compose project, the UI may be defined directly in Kotlin.
The key requirement for this experiment is that the initial screen displays the message “Hello Android!”. Keep the implementation generated by your actual project and ensure that the message shown in the running app matches the expected output.
9. Output
The application launches on an Android device and displays the greeting “Hello Android!”. The screenshot below is the screenshot supplied for this experiment.
�
Output observation: The text “Hello Android!” is visible near the top-left of the screen. The application has opened on the phone, showing the expected greeting message.
10. Project Folder and File Structure
A typical Android Studio project may have a structure similar to the following. The exact folder names and files can differ based on the template, programming language, and Android Studio version.
HelloAndroid/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/ or kotlin/
│   │       │   └── <package-name>/
│   │       │       └── MainActivity.kt or MainActivity.java
│   │       ├── res/
│   │       │   ├── layout/           # XML layouts, if used
│   │       │   ├── drawable/         # Drawable resources and images
│   │       │   ├── mipmap/           # Launcher icons
│   │       │   └── values/           # Strings, colours, themes
│   │       └── AndroidManifest.xml   # App and Activity configuration
│   └── build.gradle.kts              # App-level build configuration
├── gradle/
│   └── wrapper/                      # Gradle wrapper configuration
├── build.gradle.kts                  # Project-level build configuration
├── settings.gradle.kts               # Project and module settings
├── gradlew                            # Gradle wrapper script for Unix/macOS
├── gradlew.bat                        # Gradle wrapper script for Windows
├── screenshots/
│   ├── output.png                     # Screenshot supplied for the experiment
│   ├── test-case-1.png                # Greeting message test
│   ├── test-case-2.png                # App launch test
│   └── test-case-3-usn-name.png       # Screenshot showing student name and USN
└── README.md                          # Experiment documentation
Description of Important Files and Folders
app/: Contains the main application module.
src/main/: Contains the app's source code and resources.
MainActivity.kt / MainActivity.java: Common filenames for the Activity that controls the initial screen.
res/: Contains resources such as layouts, images, text strings, colours, and themes.
AndroidManifest.xml: Contains app configuration and component declarations.
build.gradle.kts / build.gradle: Contains build settings and dependencies.
settings.gradle.kts: Defines the project structure and included modules.
gradlew and gradlew.bat: Scripts used to run Gradle builds.
screenshots/: Stores screenshots used as evidence in this README.
README.md: Explains the aim, concepts, procedure, output, and testing of the experiment.
This is an illustrative structure. Retain the actual files created by Android Studio; do not create files solely to match this diagram if they are not required by your project.
11. Test Cases
The following test cases describe how the application should be checked. Record a test as Pass only after running it and confirming the expected result. Add the relevant screenshot for each test case.
Test Case 1: Verify the Greeting Message
Test Case ID: TC-01
Test objective: To verify that the app displays the correct greeting message.
Precondition: The application has been installed on the Android device or emulator.
Steps:
Open the application.
Observe the text displayed on the screen.
Compare the displayed text with the expected message.
Expected result: The screen displays “Hello Android!”.
Actual result: The supplied output screenshot shows “Hello Android!”.
Status: Pass if the text is displayed correctly.
�
Test Case 2: Verify Application Launch
Test Case ID: TC-02
Test objective: To verify that the application opens successfully.
Precondition: The application has been installed successfully.
Steps:
Close the application.
Open it again from the device's app screen or launcher.
Wait for the initial screen to appear.
Check whether the greeting is visible and the app remains open.
Expected result: The application launches without crashing and displays the greeting message.
Actual result: Record the result after completing this test on the device.
Status: Pass if the application opens and remains usable.
�
Test Case 3: Display Student Name and USN
Test Case ID: TC-03
Test objective: To verify that the application can display the student's name and USN as required for submission.
Precondition: The application source code or UI has been updated to display the student's correct name and USN.
Steps:
Add a text element showing the student's full name and USN to the screen.
Build and run the updated application.
Check that both details are visible and correctly spelled.
Capture a screenshot of the running application.
Save the screenshot as screenshots/test-case-3-usn-name.png.
Expected result: The application displays the student's full name and USN clearly.
Actual result: Record the result after testing.
Status: Pass only after the name and USN are visible in the screenshot.
Student details to include:
Name: YOUR FULL NAME
USN: YOUR USN
�
Important: The screenshot supplied for this README shows only “Hello Android!”; it does not show the student's name or USN. A separate screenshot must be captured after adding those details to the app. The test-case image paths for Test Cases 1–3 are placeholders until you add the corresponding screenshots.
12. Results and Discussion
The simple Android application was run and the greeting message “Hello Android!” was observed on the screen. This experiment demonstrates the basic process of building and running an Android application and verifying its visible output.
The experiment also introduces the role of Android Studio, the Activity, UI components, resources, the manifest file, and Gradle. The three proposed test cases cover the greeting text, successful application launch, and display of the student's identification details.
13. Advantages
It is a simple introduction to Android app development.
It helps beginners become familiar with Android Studio.
It demonstrates how text is displayed on a mobile screen.
It provides practice in building and running an app.
It introduces basic project documentation and screenshot-based testing.
14. Applications
A basic greeting screen can be used as:
A starting point for learning Android development.
A simple demonstration of an Android project setup.
A first screen before adding buttons, images, forms, or navigation.
A basic example for practising app execution and output verification.
15. Conclusion
The “Hello Android!” application was created and run to demonstrate the fundamentals of Android application development. The app displays the expected greeting on the device screen. The experiment provides an introduction to Android Studio, Activities, user-interface components, project structure, and testing.
For the final GitHub submission, include the actual Android project files, this README, the supplied output screenshot, and three test-case screenshots. Ensure that the third test-case screenshot clearly shows the student's name and USN.
16. GitHub Submission Checklist
[ ]
Upload the complete Android Studio project source code.
[ ]
Include this README.md in the repository root.
[ ]
Include screenshots/output.png (the supplied screenshot).
[ ]
Add screenshots/test-case-1.png.
[ ]
Add screenshots/test-case-2.png.
[ ]
Add screenshots/test-case-3-usn-name.png showing your name and USN.
[ ]
Replace YOUR FULL NAME and YOUR USN with your correct details.
[ ]
Update the folder structure if your actual project differs.
[ ]
Open the README on GitHub and verify that the output image displays correctly.
[ ]
Confirm that all three test cases have been tested and their results are accurate.
