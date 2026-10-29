# Experiment 1: Develop a Simple “Hello World” Android Application

## 1. Experiment Details

- **Experiment Number:** 1
- **Experiment Title:** Develop a Simple “Hello World” Android Application
- **Platform:** Android
- **Development Environment:** Android Studio
- **Programming Language:** Kotlin or Java, depending on the project configuration
- **Application Output:** `Hello Android!`

## 2. Aim

To develop, build, and run a basic Android application that displays the greeting message **“Hello Android!”** on a mobile screen.

## 3. Objectives

The objectives of this experiment are:

1. To understand the basic process of creating an Android application.
2. To become familiar with the Android Studio development environment.
3. To understand the purpose of an Activity in an Android application.
4. To learn how text can be displayed on an Android screen.
5. To build and run an application on an Android emulator or physical device.
6. To observe the application's output and capture a screenshot.
7. To document the application and its test cases for a GitHub submission.

## 4. Software and Hardware Requirements

### Software Requirements

- Android Studio
- Android SDK and the required build tools
- Kotlin or Java, according to the project configuration
- Gradle build system
- Android Emulator, or USB/Wireless debugging for a physical Android phone
- Git and a GitHub account for version control and submission

### Hardware Requirements

- A computer capable of running Android Studio
- An Android emulator or Android smartphone for running the application
- A USB cable if a physical phone is connected by USB

## 5. Concept and Technology Behind the Experiment

Android applications are commonly developed using Android Studio. A typical Android project contains source code, resources, a manifest file, and build configuration files. These parts work together to build and launch the app.

### 5.1 Android Studio

Android Studio is the official integrated development environment (IDE) for Android app development. It provides tools to write code, design interfaces, build projects, find errors, and run applications on emulators or physical devices.

### 5.2 Activity

An Activity represents a screen in an Android application. It controls a screen's behaviour and can display the user interface. In a simple starter project, `MainActivity` is often the first screen shown when the app launches.

### 5.3 User Interface (UI)

The user interface is the part of the application that the user sees and interacts with. In this experiment, the UI is intentionally simple: it displays the text **“Hello Android!”** against a dark background.

Depending on the Android Studio template, the screen can be created using XML layout resources, Jetpack Compose, or UI elements created in source code. The exact implementation may differ between projects.

### 5.4 AndroidManifest.xml

The manifest file describes important information about the application to the Android system. Depending on the project, it identifies the application's components and declares which Activity can be launched.

### 5.5 Gradle

Gradle is the build system used by Android projects. It helps compile the source code, process resources, and package the application so that it can be installed and run.

### 5.6 Output Screenshot

A screenshot provides visual evidence that the application has launched and displays the intended message. The screenshot included in this repository shows **“Hello Android!”** on the device screen.

## 6. Scenario Used to Demonstrate the Experiment

A student is developing their first Android application and wants to verify that the development environment is working correctly. The student creates a simple app that displays a greeting when opened.

When the application launches, the text **“Hello Android!”** appears on the screen. This small example demonstrates the basic development workflow: create a project, configure it, build it, run it on a device, and check the output.

## 7. Procedure

1. Open Android Studio on the computer.
2. Select the option to create a new Android project.
3. Choose a basic Activity template suitable for the course.
4. Enter the project name, package name, programming language, and minimum SDK required by the project.
5. Allow Android Studio to create and sync the project.
6. Open the main Activity or the screen layout used by the project.
7. Add or retain a text component that displays **“Hello Android!”**.
8. Check that the text is readable and visible on the screen.
9. Connect an Android phone or start an Android emulator.
10. Build and run the application.
11. Confirm that the app launches and the greeting appears.
12. Capture the output screenshot.
13. Add the source code, README, and screenshots to the GitHub repository.

## 8. Source Code Overview

The exact source code depends on the template selected in Android Studio. In a traditional Activity-based project, `MainActivity.kt` or `MainActivity.java` contains the screen logic, and an XML layout may define the text component. In a Jetpack Compose project, the UI may be defined directly in Kotlin.

The key requirement for this experiment is that the initial screen displays the message **“Hello Android!”**. Keep the implementation generated by your actual project and ensure that the message shown in the running app matches the expected output.

## 9. Output

The application launches on an Android device and displays the greeting **“Hello Android!”**. The screenshot below is the screenshot supplied for this experiment.

![Output screenshot showing Hello Android! on the phone screen](screenshots/output.jpeg)

**Output observation:** The text “Hello Android!” is visible near the top-left of the screen. The application has opened on the phone, showing the expected greeting message. The screen has a dark background, with the phone's status bar at the top and navigation controls at the bottom.

## 10. Project Folder and File Structure

A typical Android Studio project may have a structure similar to the following. The exact folder names and files can differ based on the template, programming language, and Android Studio version.

```text
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
│   └── output.jpeg                    # Screenshot supplied for the experiment
└── README.md                          # Experiment documentation
```

### Description of Important Files and Folders

- **`app/`:** Contains the main application module.
- **`src/main/`:** Contains the app's source code and resources.
- **`MainActivity.kt` / `MainActivity.java`:** Common filenames for the Activity that controls the initial screen.
- **`res/`:** Contains resources such as layouts, images, text strings, colours, and themes.
- **`AndroidManifest.xml`:** Contains app configuration and component declarations.
- **`build.gradle.kts` / `build.gradle`:** Contains build settings and dependencies.
- **`settings.gradle.kts`:** Defines the project structure and included modules.
- **`gradlew` and `gradlew.bat`:** Scripts used to run Gradle builds.
- **`screenshots/`:** Stores screenshots used as evidence in this README.
- **`README.md`:** Explains the aim, concepts, procedure, output, and testing of the experiment.

This is an illustrative structure. Retain the actual files created by Android Studio; do not create files solely to match this diagram if they are not required by your project.

## 11. Test Cases

The following test cases describe how the application should be checked. Record a test as **Pass** only after running it and confirming the expected result. Add the relevant screenshot for each test case.

### Test Case 1: Verify the Greeting Message

- **Test Case ID:** TC-01
- **Test objective:** To verify that the app displays the correct greeting message.
- **Precondition:** The application has been installed on the Android device or emulator.

**Steps:**
1. Open the application.
2. Observe the text displayed on the screen.
3. Compare the displayed text with the expected message.

- **Expected result:** The screen displays “Hello Android!”.
- **Actual result:** The supplied output screenshot shows “Hello Android!”.
- **Status:** Pass, based on the supplied screenshot showing the correct greeting.

### Test Case 2: Verify Application Launch

- **Test Case ID:** TC-02
- **Test objective:** To verify that the application opens successfully.
- **Precondition:** The application has been installed successfully.

**Steps:**
1. Close the application.
2. Open it again from the device's app screen or launcher.
3. Wait for the initial screen to appear.
4. Check whether the greeting is visible and the app remains open.

- **Expected result:** The application launches without crashing and displays the greeting message.
- **Actual result:** The supplied screenshot shows the app open with the greeting. A separate relaunch test has not been documented here.
- **Status:** Verify by closing and reopening the application.

### Test Case 3: Display Student Name and USN

- **Test Case ID:** TC-03
- **Test objective:** To verify that the application can display the student's name and USN as required for submission.
- **Precondition:** The application source code or UI has been updated to display the student's correct name and USN.

**Steps:**
1. Add a text element showing the student's full name and USN to the screen.
2. Build and run the updated application.
3. Check that both details are visible and correctly spelled.
4. Capture a screenshot of the running application.
5. Save the screenshot in the repository, for example as `screenshots/test-case-3-usn-name.png`.

- **Expected result:** The application displays the student's full name and USN clearly.
- **Actual result:** The supplied screenshot shows only “Hello Android!”; it does not show the student's name or USN.
- **Status:** Pending until the name and USN are added and a new screenshot is captured.

**Student details to include:**
- **Name:** YOUR FULL NAME
- **USN:** YOUR USN

> **Important:** Replace `YOUR FULL NAME` and `YOUR USN` with the correct details. The supplied screenshot does not show the student's name or USN. Capture a separate screenshot after adding those details to the app. Do not mark Test Case 3 as passed until this is completed.

## 12. Results and Discussion

The simple Android application was run and the greeting message **“Hello Android!”** was observed on the screen. This experiment demonstrates the basic process of building and running an Android application and verifying its visible output.

The experiment also introduces the role of Android Studio, the Activity, UI components, resources, the manifest file, and Gradle. The proposed test cases cover the greeting text, successful application launch, and display of the student's identification details.

## 13. Advantages

1. It is a simple introduction to Android app development.
2. It helps beginners become familiar with Android Studio.
3. It demonstrates how text is displayed on a mobile screen.
4. It provides practice in building and running an app.
5. It introduces basic project documentation and screenshot-based testing.

## 14. Applications

A basic greeting screen can be used as:

1. A starting point for learning Android development.
2. A simple demonstration of an Android project setup.
3. A first screen before adding buttons, images, forms, or navigation.
4. A basic example for practising app execution and output verification.

## 15. Conclusion

The **“Hello Android!”** application was created and run to demonstrate the fundamentals of Android application development. The app displays the expected greeting on the device screen. The experiment provides an introduction to Android Studio, Activities, user-interface components, project structure, and testing.

For the final GitHub submission, include the actual Android project files, this README, the supplied output screenshot, and any additional test-case screenshots required by your instructor. Ensure that the third test-case screenshot clearly shows the student's name and USN if this is part of the submission requirements.

## 16. GitHub Submission Checklist

- [ ] Upload the complete Android Studio project source code.
- [ ] Include this `README.md` in the repository root.
- [ ] Include `screenshots/output.jpeg` (the supplied screenshot).
- [ ] Add a screenshot for Test Case 1 if required.
- [ ] Add a screenshot for Test Case 2 if required.
- [ ] Add `screenshots/test-case-3-usn-name.png` showing your name and USN.
- [ ] Replace `YOUR FULL NAME` and `YOUR USN` with your correct details.
- [ ] Update the folder structure if your actual project differs.
- [ ] Open the README on GitHub and verify that the output image displays correctly.
- [ ] Confirm that all test cases have been tested and their results are accurate.
