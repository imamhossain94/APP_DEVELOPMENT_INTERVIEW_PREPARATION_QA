<h2 align="center">APP DEVELOPMENT INTERVIEW PREPARATION QA</h2>

<h2 align="center">What is Android?</h2>

<b>Android is an open-sourced operating system that is used on mobile devices, such as mobiles and tablets. The Android application executes within its own process and its own instance of Dalvik Virtual Machine(DVM) or Android RunTime(ART).</b>

<h2 align="center">What are the features of Android architecture?</h2>
<body>
<table width="100%">
<tr>
<td width="100%" >
<img src="https://github.com/ahoteshanul/APP_DEVELOPMENT_INTERVIEW_PREPARATION_QA/blob/main/IMAGES/Android%20architecture.png" alt="LOADING" width="100%" height="100%" >
</td>
</tr>
  
<b>The five layers present in the Android stack are:</b>

- Linux Kernel - It is responsible for device drivers, device management, memory management, power management, and resource access.
- Libraries - There are a set of libraries having open-source Web browser engine WebKit, well-known library libc, libraries to play and record audio and video, SQLite database for sharing of application data and storage, SSL libraries for internet security, etc.
- Android Runtime - There are core libraries along with DVM (Dalvik Virtual Machine) or ART(Android RunTime) as runtime which is helpful for running an Android application. DVM is optimized for mobile devices. DVM provides fast performance and consumes less memory. Replacing DVM, ART(Android RunTime) virtual machine was introduced to execute android apps from Android lollipop 5.0 version (API level 21).
- Android Framework - It consists of Android APIs like UI (User Interface), resources, content providers (data), locations, telephony, and package managers. It provides interfaces and classes for the development of Android applications.
- Android Applications - Applications like home, games, contacts, settings, browsers, etc. uses the Android framework that will make use of Android runtime and libraries.
