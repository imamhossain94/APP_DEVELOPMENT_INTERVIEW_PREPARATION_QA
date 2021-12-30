<h2 align="center">APP DEVELOPMENT INTERVIEW PREPARATION QA</h2>

<h2 align="center">What is Android?</h2>

<b>Android is an open-sourced operating system that is used on mobile devices, such as mobiles and tablets. The Android application executes within its own process and its own instance of Dalvik Virtual Machine(DVM) or Android RunTime(ART).</b>

<h2 align="center">What are the features of Android architecture?</h2>

<!-- <html>
<body>
<table width="100%">
<tr>
<td width="100%" >
<img src="https://github.com/ahoteshanul/APP_DEVELOPMENT_INTERVIEW_PREPARATION_QA/blob/main/IMAGES/Android%20architecture.png" alt="LOADING" width="100%"  >
</td>
</tr>
</html> -->
    
<b>The five layers present in the Android stack are: </b>

- <b> Linux Kernel: </br> It is responsible for device drivers, device management, memory management, power management, and resource access. </b>
- <b> Libraries: </br> There are a set of libraries having open-source Web browser engine WebKit, well-known library libc, libraries to play and record audio and video, SQLite database for sharing of application data and storage, SSL libraries for internet security, etc. </b>
- <b> Android Runtime: </br> There are core libraries along with DVM (Dalvik Virtual Machine) or ART(Android RunTime) as runtime which is helpful for running an Android application. DVM is optimized for mobile devices. DVM provides fast performance and consumes less memory. Replacing DVM, ART(Android RunTime) virtual machine was introduced to execute android apps from Android lollipop 5.0 version (API level 21). </b>
- <b> Android Framework: </br> It consists of Android APIs like UI (User Interface), resources, content providers (data), locations, telephony, and package managers. It provides interfaces and classes for the development of Android applications. </b>
- <b> Android Applications: </br>  Applications like home, games, contacts, settings, browsers, etc. uses the Android framework that will make use of Android runtime and libraries. </b>

<h2 align="center">List the languages used to build Android.</h2>
<b>Java, Kotlin, C#, Python </br>
Other languages which can be used in Android development are C++, HTML 5. C4droid, CppDroid, AIDE, etc. are IDE’s for C++. Acode, spck code editor, etc. are examples of IDE’s used with HTML.</b>

<h2 align="center">What is an activity?</h2>

<b>Activity in java is a single screen that represents GUI(Graphical User Interface) with which users can interact in order to do something.</b>

<h2 align="center">What is a service in Android?</h2>

<b> Service is an application component that facilitates an application to run in the background in order to perform long-running operations without user interaction. A service can run continuously in the background even if the application is closed or even after the user switches to another application. </b>

<h2 align="center">Differentiate Activities from Services.</h2>

| Activities  | Services |
| ------------- | ------------- |
| They are designed to run in the foreground.  | These are mainly designed to run in the background. Foreground services are also available  |
| Used when the user interface is necessary.  | Used when the user interface is not necessary.  |
| They are dependent.  | They act independently.  |

<h2 align="center">What is Google Android SDK? Which are the tools placed in Android SDK?</h2>

<b>The Google Android SDK is a toolset used by developers to write applications on Android-enabled devices.</b>

The tools placed in Android SDK are given below:

- Android Emulator - Android Emulator is a software application that simulates Android devices on your computer so that you can test the application on a variety of devices and Android API levels without having each physical device.
- DDMS(Dalvik Debug Monitoring Services) - It is a debugging tool from the Android software development kit (SDK) which provides services like message formation, call spoofing, capturing screenshots, etc.
- ADB(Android Debug Bridge) - It is a command-line tool used to allow and control communication with the emulator instance.
- AAPT(Android Asset Packaging Tool) - It is a build tool that gives the ability to developers to view, create, and update ZIP-compatible archives (zip, jar, and apk).

<h2 align="center">What is the use of Bundle in Android?</h2>

<b>Bundles are used to pass the required data between various Android activities. These are like HashMap that can take trivial data types. Below code shows how to transfer a piece of data by using bundle:</b>
```
Bundle b=new Bundle();
b.putString("Email","abc@xyz.com");
i.putExtras(b); // where i is intent
```

<h2 align="center">Abbreviation</h2>

- <b> ART: Android RunTime</b>
- <b> DVM: Dalvik Virtual Machine</b>
- <b> UI: User Interface</b>
- <b> GUI: Graphical User Interface</b>
- <b> DDMS: Dalvik Debug Monitoring Services</b>
- <b> AAPT: Android Asset Packaging Tool</b>
