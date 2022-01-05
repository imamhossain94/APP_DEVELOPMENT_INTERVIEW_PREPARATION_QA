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

```java
Bundle b=new Bundle();
b.putString("Email","abc@xyz.com");
i.putExtras(b); // where i is intent
```
<h2 align="center">What is an Adapter in Android?</h2>

<b>An adapter in Android acts as a bridge between an AdapterView and the underlying data for that view. The adapter holds the data and sends the data to the adapter view, the view can take the data from the adapter view and shows the data on different views like a spinner, list view, grid view, etc.</b>

<h2 align="center">What is AAPT?</h2>

<b>AAPT stands for Android Asset Packaging Tool. It is a build tool that gives the ability to developers to view, create, and update ZIP-compatible archives (zip, jar, and apk). It parses, indexes, and compiles the resources into a binary format that is optimized for the platform of Android..</b>

<h2 align="center">What is portable Wi-Fi hotspot?</h2>

<b>Portable Wi-Fi Hotspot permits you to share your mobile internet connection with other wireless devices.</b>

<h2 align="center">What is Android Debug Bridge(ADB)?</h2>

<b>Android Debug Bridge is a command-line tool used to allow and control communication with an emulator instance. It gives the power for developers to execute remote shell commands to run applications on an emulator.</b>

<h2 align="center">What is DDMS?</h2>

<b> DDMS(Dalvik Debug Monitor Server) is a debugging tool in the Android platform. It gives the following list of debugging features:<b/>

- Port forwarding services.
- Thread and heap information.
- Logcat.
- Screen capture on the device.
- Network traffic tracking.
- Incoming call and SMS spoofing.
- Location data spoofing.

<h2 align="center">What is AIDL? Which data types are supported by AIDL?</h2>
<b>AIDL(Android Interface Definition Language) is a tool that handles the interface requirements between a client and a service for interprocess communication(IPC) to communicate at the same level.</b>
<br>
<b>The process involves dividing an object into primitives that are understood by the Android operating system. Data Types supported by AIDL is as follows:</b>

- String
- List
- Map
- CharSequence
- Java data types (int, long, char, and boolean)

<h2 align="center">What is the life cycle of Android activity?</h2>
    

- OnCreate(): <br>It is called when activity is created. Using this, the views are created and data is collected from bundles.
- OnStart(): <br>It is called if the activity is becoming visible to the user. It may be succeeded by onResume() if the activity comes to the foreground, or onStop() if it becomes hidden.
- OnResume(): <br>It is called when the activity will start an interaction with the user.
- OnPause(): <br>This is called when the activity is moving to the background but hasn’t been killed yet.
- OnStop(): <br>This is called when an activity is no longer visible to the user.
- OnDestroy(): <br>This is called when the activity is finished or destroyed.
- OnRestart(): <br>This is called after the activity has been stopped, prior to it being started again.


<h2 align="center">Explain Sensors in Android.</h2>
    
Android-based devices have a collection of built-in sensors in them, which measure certain parameters like motion, orientation, and many more through their high accuracy. The sensors can be both hardware and software based on nature. There are three prominent categories of sensors in Android devices.
<br>They are:

- Position Sensor: <br>It is used for measuring the physical position of the Android device. This has orientation sensors and magnetometers.
- Motion Sensors: <br>These sensors consist of gravity, rotational activity, and acceleration sensors which measure the rotation of the device or the acceleration, etc.
- Environmental Sensor: <br>It includes sensors that measure temperature, humidity, pressure, and other environmental factors.

<h2 align="center">Explain the dialog boxes supported on Android.</h2>
    
Android supports four dialog boxes. They are:
    
- AlertDialog:
        <br>The AlertDialog supports 0-3 buttons, along with a list of selectable items such as checkboxes and radio buttons.
        It is used when you want to ask the user about taking a decision between yes or no in response to any particular action taken by the user, by remaining in the same activity and without changing the screen.
- DatePickerDialog:
        <br>It is used for selecting the date by the user.
- TimePickerDialog:
        <br>Used for selecting the time by the user.
- ProgressDialog:
        <br>It is an extension of the AlertDialog and is used to display a progress bar. It also supports the addition of buttons.
        This class was deprecated in API level 26 because it prevents the user from interacting with the application. Instead of this class, we can use a progress indicator such as ProgressBar, which can be embedded in the user interface of your application.

<h2 align="center">What is AndroidManifest.xml file and why do you need this?</h2>

- The AndroidManifest.xml file contains information regarding the application that the Android system must know before the codes can be executed.
- This file is essential in every Android application.
- It is declared in the root directory.
- This file performs several tasks such as:
- Providing a unique name to the java package.
- Describing various components of the application such as activity, services, and many more.
- Defining the classes which will implement these components.

<h2 align="center">What is an intent?</h2>
    
An intent is a messaging object that is used to request an action from other components of an application. It can also be used to launch an activity, send SMS, send an email, display a web page, etc.

It shows notification messages to the user from within an Android-enabled device. It alerts the user of a particular state that occurred. There are two types of intents in Android:

- Implicit Intent- Used to invoke the system components.
- Explicit Intent- Used to invoke the activity class.

<h2 align="center">Mention the difference between class, file and activity in Android?</h2>
    
The difference between them is as follows:

 
- Class is a compiled form of a .java file that Android uses to produce an executable .apk file.
- A file is a block of arbitrary information or resources used for storing information. It can be of any file type.
- Activity is a single screen that represents GUI(Graphical User Interface) with which users can interact in order to do something like dial the phone, view email, etc.

<h2 align="center">What is a Toast? Write its syntax.</h2>
    
Toast is a message that pops up on the screen. It is used to display the message regarding the status of the operation initiated by the user and covers only the expanse of space required for the message while the user’s recent activity remains visible and interactive.

Toast notification automatically fades in and out and it does not accept interaction events.

```java
Toast.makeText(ProjectActivity.this, "Your message here", Toast.LENGTH_LONG).show();
```

<h2 align="center">What is context?</h2>

The context in Android is the context of the current state of the application or object. The context comes with services like giving access to databases and preferences, resolving resources, and more.
There are two types of context. They are:
    
<h3 align="center">Activity context</h3>

- This activity context is attached to the lifecycle of an activity.
- The activity context can be used when you are passing the context in the scope of an activity or you need the context whose lifecycle is attached to the context of the activity.
    
<h3 align="center">Application context:</h3>

- This application context is attached to the lifecycle of an application.
- The application context should be used where you need a context whose lifecycle is separate from the current context or when you are passing a context beyond the scope of activity.

<h2 align="center">Abbreviation</h2>
    
The difference between the implicit and explicit Intents are given below:

<h3 align="center">Explicit Intent:</h3>

An Explicit Intent is where you inform the system about which activity should handle this intent. Here target component is defined directly in the intent.
    
```java
Intent i = new Intent(this, Activitytwo.class); #ActivityTwo is the target component
i.putExtra("Value1","This is ActivityTwo"); 
i.putExtra("Value2","This Value two for ActivityTwo"); 
startactivity(i);
```
<h3 align="center">Implicit Intent:</h3>

An Implicit Intent permits you to declare the action you want to carry out. Further, the Android system will check which components are registered to handle that specific action based on intent data. Here target component is not defined in the intent.
    
```java
Intent i = new Intent(ACTION_VIEW,Uri.parse("http://www.interview bit.com")); 
startActivity(i);
```
<h2 align="center">What is ANR in Android? What are the measures you can take to avoid ANR?</h2>

ANR(Application is Not Responding) is a dialog box that appears when the application is not responding. This ANR dialogue is displayed whenever the main thread within an application has been unresponsive for a long time under the following conditions:
- When there is no response to an input event even after 5 seconds.
- When a broadcast receiver has not completed its execution within 10 seconds.

Following measures can be taken to avoid ANR:
- An application should perform lengthy database or networking operations in separate threads to avoid ANR.
- For background task-intensive applications, you can lessen pressure from the UI thread by using the IntentService.

<h2 align="center">What are the troubleshooting techniques you can follow if an application is crashing frequently?</h2>
    
If an Android application is crashing frequently, you can follow the below-given techniques:
    
<h3 align="center">Compatibility Check:</h3>
It is not possible to test an application for all kinds of devices and operating systems. There might be a possibility that an application is not compatible with your OS.

<h3 align="center">Memory Management:</h3>

- Some apps run perfectly on one mobile device but might crash on other devices. This is where processing power, memory management, and CPU speed are considered.
- As there is a limited amount of memory space on mobile devices, you can free up memory space for the application to function properly.
- If an application is frequently crashing, you can delete the application’s data, which will clear its cache memory and allow some free space on your device and might boost the app’s performance.

<h2 align="center">Explain different launch modes in Android.</h2>
    
The different launch modes in Android are given below:
<br>
`Standard:`

- This launch mode generates an activity’s new instance in the task from which it originated.
- It is possible to create several instances for the same activity.
- For Example, suppose our current stack is A -> B -> C. Now, if we launch activity B again with the “standard” launch mode, then the new stack will be A -> B -> C -> B.

`SingleTop:`

- This launch mode is similar to the Standard launch mode except if there exists an activity’s previous instance on the top of the stack, then a new instance will not be created.
- But the intent will be sent to the activity’s existing instance.
- For example, suppose our current stack is A -> B -> C. Now, if we launch the activity B again with “singleTop” launch mode,then the new stack will be A -> B -> C -> B.
  Consider another example, where the current stack is A -> B -> C. Now, if we launch activity C again with the “singleTop” launch mode, then the stack will remain the same    i.e., A -> B -> C. The intent will be passed to the onNewIntent() method.

`SingleTask:`

- This launch mode will create a new task and push a new instance to the task as the root.
- For example, suppose our current stack is A -> B -> C -> D. Now, if we launch activity B again with the “singleTask” launch mode, then the new stack will be A -> B. Here, a callback has been received on the old instance and C and D activities are destroyed.

 `SingleInstance:`
 
- This launch mode is similar to the SingleTask launch mode. But the system doesn’t support launching any new activities in the same task.
- In a situation where the new activity is launched, it is launched in a separate task.
- For example, Suppose our current stack is A -> B -> C. Now, if we launch the activity D with the “singleInstance” launch mode, then there will be two stacks:
       <br>A -> B -> C 
        <br>D, If you call activity E, then it will be added to the first stack.
        <br>A -> B -> C -> E
        <br>D<br>

Again if you Call the activity D, then it will call the same activity from the 2nd stack and pass the intent to onNewIntent().
    
<h2 align="center">What are containers?</h2>
    
Containers carry objects and widgets together, based on which specific items are required and in what particular arrangement is needed. Containers may hold labels, buttons, fields, or even child containers, etc. For example, if you want a form with fields on the left and labels on the right, you will need a container. If you want the OK and Cancel buttons to be below the rest of the form, next to one another, and flush to the right side of the screen, you will need a container. If you have several widgets, you will need a container to have a root element to place the widgets inside.

Android provides a collection of view classes that serve as containers for views. These container classes are called layouts, which are defined in the form of XML files that cannot be changed by our code during execution. The layout managers provided by Android SDK are LinearLayout, RelativeLayout, FrameLayout, AbsoluteLayout, GridLayout, and TableLayout.

<h2 align="center">What is the role of Dalvik in Android development?</h2>
    
Dalvik serves as a virtual machine, and it is responsible for running every Android application. Because of Dalvik, a device will have the ability to execute multiple instances of virtual machines efficiently through better memory management.

<h2 align="center">What are broadcast receivers? How is it implemented?</h2>
    
A broadcast receiver is a mechanism used for listening to system-level events like listening for incoming calls, SMS, etc. by the host application. It is implemented as a subclass of BroadcastReceiver class and each message is broadcasted as an intent object.
 
```java
public class MyReceiver extends BroadcastReceiver 
{
    public void onReceive(context,intent){}
}
```
 
<h2 align="center">Explain in detail about the important file and folders used when you create a new Android application.</h2>

It describes the basic characteristics of the application and defines each of its components.
<br>
`java:`
- This contains the .java source files and .kt(source code written in Kotlin) source files of your project. By default, it includes a MainActivity.java or MainActivity.kt source file.
- You create all the activities which have .java and .kt extensions under this file and also it includes all the code behind the application.
`res:`
- It is used to store the values for the resources that are used in various Android projects to include features of color, styles, dimensions, etc.
- It is a directory for files like styles.xml, strings.xml, colors.xml, dimens.xml, etc.

`Scripts:`<br>
 This is an auto-generated file that consists of compileSdkVersion, buildToolsVersion, minSdkVersion, targetSdkVersion, applicationId, versionCode, and versionName. For example, build.gradle is a script file placed in the root project directory, defines build configurations that will be applied to all modules in your project.
    
<h2 align="center">What is the difference between Serializable and Parcelable? Which is the best approach in Android?</h2>

While developing applications usually it needs to transfer data from one activity to another. This data needs to be added into a corresponding intent object. Some additional actions are required to make the data suitable for transfer. For doing that the object should be either serializable or parcelable.

`Serializable:`
- Serializable is a standard Java interface. In this approach, you simply mark a class Serializable by implementing the interface and java will automatically serialize it.
- Reflection is used during the process and many additional objects are created. This leads to plenty of garbage collection and poor performance.
<br>
`Parcelable:`
- Parcelable is an Android-specific interface. In this approach, you implement the serialization yourself.
- Reflection is not used during this process and hence no garbage is created.
- Parcelable is far more efficient than Serializable since it gets around some problems with the default Java serialization scheme. Also, it is faster because it is optimized for usage on the development of Android, and shows better results.


<h2 align="center">What database is used in Android? How it is different from client-server database management systems?</h2>
    
SQLite is the open-source relational database used in Android. The SQLite engine is serverless, transactional, and also self-contained. Instead of the client-server relationship of most database management systems, the SQLite engine is integrally linked with the application. The library can be called dynamically and it can make use of simple function calls that reduce latency in database access.

<h2 align="center">What are the differences between Service and Thread?</h2>

The main difference between Service and Thread is given below:

| Service  | Thread |
| ------------- | ------------- |
| Service is an application component that facilitates an application to run in the background in order to perform long-running operations without user interaction.  | A Thread is a concurrent unit of execution.  |
| It exposes few functionalities to other applications by calling Context.bindService().  | Google has brought in handlers and loopers into threads.  |
| When an application is killed, service is not killed.  | When an application is killed, the thread is killed.  |

<h2 align="center">Abbreviation</h2>

Content provider is one of the primary building blocks of Android applications, which manages access to a central repository of data. It acts as a standard interface that connects data in one process with code running in another process. So it can be used to share the data between different applications.

They are responsible for encapsulating the data and providing mechanisms for defining data security. It is implemented as a subclass of ContentProviderclass and must implement a set of APIs that will enable other applications to perform transactions.

```java
public class MyContentprovider extends ContentProvider 
{
 public void onCreate(){}
}
```
<h2 align="center">What is the significance of the .dex file?</h2>
    
Android programs are compiled into a .dex file (Dalvik Executable file) by DVM, which are then zipped into a .apk file on the device. .dex files are created by translating compiled applications written in java. .dex is a format that is optimized for effective storage and memory-mappable executions.

<h2 align="center">What is the difference between compileSdkVersion and targetSdkVersion?</h2>
    
`compileSdkVersion:`

- The compileSdkVersion is the version of API the application is compiled against. You can use Android API features involved in that version of the API (as well as all previous versions).
- For example, if you try and use API 15 features but set compileSdkVersion to 14, you will get a compilation error. If you set compileSdkVersion to 15 you can still run the app on an API 14 device as long as your app’s execution paths do not attempt to invoke any APIs specific to API 15.

`targetSdkVersion:`
<br>
- The targetSdkVersion indicates that you have tested your app on (presumably up to and including) the version you specify. This is like a certification or sign-off you are giving the Android OS as a hint to how it should handle your application in terms of OS features.
- For example, setting the targetSdkVersion value to “11” or higher permits the system to apply a new default theme (Holo) to the application when running on Android 3.0 or higher. It also disables screen compatibility mode when running on larger screens (because support for API level 11 implicitly supports larger screens).

<h2 align="center">Explain about java classes related to the use of sensors on Android.</h2>

Android sensor API provides many classes and interface for the use of sensors on Android. The important classes and interfaces of sensor API are given below:

- `Sensor class:` This class helps you to create an instance of a specific sensor. It provides methods that let you determine a sensor’s capabilities.
- `SensorManager class:` This class is used to create an instance of the sensor service. It provides methods to access and list sensors, to register and unregister sensor listeners, etc.
- `SensorEvent class:` This Java class is used to create a sensor event object. It provides information about the sensor event including raw sensor data, the accuracy of data, type of sensor, timestamp of event, etc.
- `SensorEventListener interface:` This interface is used to create two callback methods that receive sensor event notifications when sensor value changes or when sensor accuracy changes. Those two methods are `void onAccuracyChanged(Sensor sensor, int accuracy)` which is called when sensor accuracy is changed and
 `void onSensorChanged(SensorEvent event)` which is called when sensor values are changed.

<h2 align="center">What is JobScheduler?</h2>

The JobSchedular API is used for scheduling different types of jobs against the framework that will be executed in your app’s own process. This allows your application to perform the given task while being considerate of the device’s battery at the cost of timing control.

The JobScheduler supports batch scheduling of jobs. The Android system can combine jobs for reducing battery consumption. JobManager automatically handles the network unreliability so it makes handling uploads easier.

Here is some example of the situation where you would use this job scheduler:

- Tasks that should be done when the device is connected to a power supply.
- Tasks that require a Wi-Fi connection or network access.
- Tasks that should run on a regular basis as batch where the timing is not critical.

<h2 align="center">Abbreviation</h2>
    
- <b> ART: Android RunTime</b>
- <b> DVM: Dalvik Virtual Machine</b>
- <b> UI: User Interface</b>
- <b> GUI: Graphical User Interface</b>
- <b> DDMS: Dalvik Debug Monitoring Services</b>
- <b> AAPT: Android Asset Packaging Tool</b>
- <b> ADB: Android Debug Bridge</b>
    
| Code name  | Version numbers | API level  | Release date |
| ------------- | ------------- | ------------- | ------------- |
| No codename  | 1.0  | 1  | September 23, 2008  |
| No codename  | 1.1  | 2  | February 9, 2009  |
| Cupcake  | 1.5  | 3  | April 27, 2009  |
| Donut  | 1.6  | 4  |  	September 15, 2009  |
| Eclair  | 2.0 - 2.1 | 5 - 7  | October 26, 2009  |
| Froyo  | 2.2 - 2.2.3  | 8  | May 20, 2010  |
| Gingerbread  | 2.3 - 2.3.7  |  	9 - 10  | December 6, 2010  |
| Honeycomb  | 3.0 - 3.2.6  | 11 - 13  | February 22, 2011  |
| Ice Cream Sandwich  | 4.0 - 4.0.4  | 14 - 15  | October 18, 2011  |
| Jelly Bean  | 4.1 - 4.3.1  | 16 - 18  | July 9, 2012  |
| KitKat  | 4.4 - 4.4.4  | 19 - 20  | October 31, 2013  |
| Lollipop  | 5.0 - 5.1.1  | 21- 22  | November 12, 2014  |
| Marshmallow  | 6.0 - 6.0.1  | 23  | October 5, 2015  |
| Nougat  | 7.0  | 24  | August 22, 2016  |
| Nougat  | 7.1.0 - 7.1.2  | 25  | October 4, 2016  |
| Oreo  | 8.0  | 26  | August 21, 2017  |
| Oreo  | 8.1  | 27  | December 5, 2017  |
| Pie  | 9.0  | 28  | August 6, 2018  |
| Android 10  | 10.0  | 29  | September 3, 2019  |
| Android 11  | 11  | 30  | September 8, 2020  |
