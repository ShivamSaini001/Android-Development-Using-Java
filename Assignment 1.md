# Assignment - 1

## Ques 1. Discuss the evolution of the Android Operating System. Explain the history, major milestones, and the key features that have made Android the most widely used mobile operating system.


### History, Major Milestones, and Key Features of Android

- Android was originally developed by **Android Inc.**, a company founded in **2003** by **Andy Rubin** and others.

- **In 2005, Google acquired Android Inc.** Google continued developing Android as an open mobile platform.

- In **2007**, Google and several technology companies created the **Open Handset Alliance (OHA)** to develop open standards for mobile devices.

- The first commercial Android smartphone was the **HTC Dream**, also known as the **T-Mobile G1**, released in **2008**.

- It is based on the **Linux kernel** and is mainly used in smartphones and tablets. Today, Android is also used in smart TVs, smartwatches, cars, and other smart devices.


### Evolution of Android Operating System

Android is a **mobile operating system developed mainly for smartphones, tablets, TVs, watches, cars, and other smart devices.** It has evolved over the years by adding better performance, security, user interface, and new features.

| **Android Version** | **Release Year** | **Major Features / Improvements** |
|---|---:|---|
| **Android 1.0** | 2008 | The First commercial Android version release in 2008. It came with basic features such as: Gmail, Google Maps, YouTube, Web browser, Android Market for downloading applications. It was mainly designed for smartphones. |
| **Android 1.5 Cupcake** | 2009 | Android started using **dessert** names for its versions. Important features: On-screen keyboard, Widgets, Video recording, Better user interface. |
| **Android 1.6 Donut** | 2009 | Improved support for different screen sizes and resolutions, Better search functionality, Improved Android Market. |
| **Android 2.0/2.1 Éclair** | 2009 | Improved user interface, Multiple Google accounts could be used, Improved Google Maps and navigation, Live wallpapers were introduced. |
| **Android 2.2 Froyo** | 2010 | Faster performance, Wi-Fi hotspot, improved browser, app-to-SD support |
| **Android 2.3 Gingerbread** | 2010 | Better keyboard, power management, NFC support, improved gaming |
| **Android 3.0 Honeycomb** | 2011 | Designed for tablets, improved multitasking, tablet UI |
| **Android 4.0 Ice Cream Sandwich** | 2011 | Combined smartphone and tablet versions into one platform, Face Unlock, improved notifications and multitasking. |
| **Android 4.1–4.3 Jelly Bean** | 2012–2013 | Smoother interface, Google Now, better notifications and performance |
| **Android 4.4 KitKat** | 2013 | Better performance on low-memory devices, immersive full-screen mode |
| **Android 5.0 Lollipop** | 2014 | Material Design, improved notifications, ART runtime, better battery management |
| **Android 6.0 Marshmallow** | 2015 | Runtime permissions, Doze mode, fingerprint support, better battery life |
| **Android 7.0 Nougat** | 2016 | Introduced **split-screen multitasking**, improved notifications, Vulkan support |
| **Android 8.0 Oreo** | 2017 | Introduced **Picture-in-Picture mode**, notification channels, background activity restrictions |
| **Android 9 Pie** | 2018 | Introduced gesture-based navigation., Adaptive Battery, Digital Wellbeing |
| **Android 10** | 2019 | Dark Mode, improved privacy, gesture navigation, better permission controls |
| **Android 11** | 2020 | Introduced **built-in screen recording**, conversation notifications, improved permissions and 5G support |
| **Android 12** | 2021 | Material You, major UI redesign, Privacy Dashboard, camera/microphone indicators |
| **Android 13** | 2022 | Per-app languages, notification permissions, improved privacy and tablet support |
| **Android 14** | 2023 | Better battery, accessibility, privacy, security and large-screen support |
| **Android 15** | 2024 | Improved security, privacy, multitasking, foldable and large-screen support |
| **Android 16** | 2025 | Improved security, performance, adaptive UI, large-screen support and modern device features |


### Key Features That Made Android Popular

**1. Open-Source Platform:** Android is based on the Android Open Source Project (AOSP). This allows manufacturers and developers to use and modify the Android platform.
This helped many companies create their own Android-based devices.

**2. Support for Many Devices:** Android is not limited to one company or one type of device.  
It is used by manufacturers such as:  
- Samsung
- Xiaomi
- OnePlus
- Motorola
- Oppo
- Vivo
- Google

This created a huge variety of Android devices at different prices.

**3. Google Play Store:** The Google Play Store provides millions of applications and games. Users can easily download:

**4. Customization:** Android provides significant customization options.  
Users can change:
- Wallpapers
- Widgets
- Launchers
- Themes
- Icons
- Home-screen layouts
- Default applications

**5. Affordable Devices:** 
This allowed Android to reach users across different income levels and markets.

**6. Multitasking:** Android supports running multiple applications and switching between them.  
Modern Android also supports features such as:
- Split-screen mode
- Picture-in-picture
- Floating windows on some devices
- Multiple applications running in the background

**7. Strong Google Ecosystem:** Android works closely with Google's services, including:
- Google Search
- Google Maps
- Gmail
- Google Photos
- YouTube
- Google Drive
- Google Assistant

**8. Hardware Support:** 
Android supports many types of hardware, including:
- Touchscreens
- Cameras
- GPS
- Bluetooth
- Wi-Fi
- NFC
- Fingerprint sensors
- Face recognition
- 5G
- Foldable displays

**9. Developer-Friendly Platform:** Android provides developers with tools and frameworks for building applications.  
Developers can use technologies such as:
- Android Studio
- Kotlin
- Java
- Android SDK
- Jetpack libraries



## Ques 2. Explain the Android Architecture with a neat labeled diagram. Describe the functions of each layer and explain how these layers interact to execute an Android application.

Android architecture is a **layered software architecture**. Each layer performs a specific job and works with the layers above and below it.

<img src = "./assets/Android Architecture.png" alt = "Android Architecture">


### Layers of Android architecture

Android Architecture is divided into six main layers--

**1. Applications Layer:** 
- This is the **top layer** of Android architecture. It contains applications that users directly interact with.  
- Applications can be **pre-installed system applications** or applications installed by the user.  
- It provides the user interface.  
- It allows users to perform different tasks.  
- The Applications layer provides the actual functionality that the user needs.  
- *For example:*  

          User 
            ⬇
        Click on Camera App  
            ⬇
        Camera Application open  

    The camera application doesn't directly control the camera hardware. It uses Android's lower layers to access it.


**2. Application Framework Layer:** 
- The Application Framework provides a set of **APIs and system services** that applications use to perform common operations.
- Instead of every application creating its own system services, Android provides these services through the framework.
- This layer provides **ready-made services** to applications.  
For example, suppose your app wants to:
    - Open a camera
    - Show a notification
    - Find your location
    - Create a window
    - Manage an activity

- Instead of building everything from scratch, the app asks Android's Application Framework.  
For example:

        Camera App
            ↓
        Camera-related Android APIs/services
            ↓
        Camera Hardware



**3. Android Runtime and Native Libraries** 

This layer contains two important parts:--

A) Android Runtime (ART)  
B) Native Libraries

**A) Android Runtime (ART):** 
- ART stands for Android Runtime.
- Its main job is to **execute Android application code.**
- Android applications are commonly developed using **Java or Kotlin**. 
- Their code is compiled into Android's executable format, including **DEX bytecode**, which ART executes.
- It Provides core runtime libraries, Manages memory, and Performs garbage collection.

- **Simple flow**

        Java / Kotlin Code
            ↓
        Compilation
            ↓
        DEX Bytecode
            ↓
            ART
            ↓
        Application Runs

**B. Native Libraries:** 
- Android also contains many libraries written mainly in C/C++.  
- These libraries provide low-level functionality to the Android system and applications.

- **Examples**  

    | Library |	Function |
    |---------|----------|
    | SQLite |	Provides database functionality |
    | OpenGL ES |	Provides graphics functionality |
    | Media Framework |	Handles audio and video |
    | SSL/TLS libraries |	Provide secure communication |
    | Native C/C++ libraries |	Provide various low-level functions |


- **Examples**  
    If an application needs to store data locally:

        Application
            ↓
        Android Framework
            ↓
        SQLite
            ↓
        Local Database


**4. Hardware Abstraction Layer (HAL):**  

- The Hardware Abstraction Layer (HAL) provides a **standard interface** between Android's higher-level software and hardware-specific implementations.
- Different manufacturers use different hardware.  
  **For example:**

        Phone A → Camera Hardware A
        Phone B → Camera Hardware B
        Phone C → Camera Hardware C


- **Examples of HAL**  
    - Camera HAL
    - Audio HAL
    - Sensors HAL
    - Bluetooth-related hardware interfaces
    - Wi-Fi-related hardware interfaces

- **Example**

        Camera Application
                ↓
        Application Framework
                ↓
            Camera HAL
                ↓
        Camera Hardware


**5. Linux Kernel Layer:**

- The Linux Kernel is the foundation of Android's operating system.
- It is responsible for managing the device's core resources and providing important low-level system functionality.

- **Major Functions**
    - **Process Management:** It manages running processes and helps the system decide how CPU resources are used.
    - **Memory Management:** It manages RAM and controls how memory is allocated to processes.
    - **Device Drivers:** Drivers allow the operating system to communicate with hardware.  
    **Examples:**
        - Camera driver
        - Display driver
        - Audio driver
        - Wi-Fi driver
        - Bluetooth driver
    
    - **Power Management:** It manages power consumption to help improve battery life.

    - **Networking:** It provides networking functionality for Wi-Fi, mobile networks, and other communication.

    - **Security:** It provides important security mechanisms that help isolate applications and protect system resources.

**6. Hardware Layer:**

- The Hardware Layer represents the physical components of an Android device.
- **Examples include:**
    - CPU
    - RAM
    - Camera
    - Display
    - Microphone
    - Speaker
    - GPS
    - Wi-Fi hardware
    - Bluetooth hardware
    - Storage


## Ques 3. Android applications are composed of four major application components. Explain Activity, Service, Broadcast Receiver, and Content Provider with suitable real-life examples and practical use cases.

### Four Major Components of Android Applications

An Android application is mainly made up of four major components:
1. Activity
2. Service
3. Broadcast Receiver
4. Content Provider

Each component has a different purpose.

**1. Activity:** 
- An Activity represents a **screen** or **user interface** of an Android application.
- Whenever you open a screen in an app and interact with buttons, text fields, images, etc., you are usually interacting with an Activity.

- **Real-life example**

    Think about a restaurant.

        Restaurant App
            ↓
        ┌─────────────────┐
        │    Home Screen  │ ← Activity
        └─────────────────┘
            ↓
        ┌─────────────────┐
        │  Food Details   │ ← Activity
        └─────────────────┘
            ↓
        ┌─────────────────┐
        │   Order Screen  │ ← Activity
        └─────────────────┘


- **Practical use cases:** Activity is used for--
    - Login screen
    - Registration screen
    - Home screen
    - Product details
    - Shopping cart
    - Payment screen
    - Settings screen

- **Example:** In a shopping application--

        Login Activity
            ↓
        Home Activity
            ↓
        Product Activity
            ↓
        Cart Activity
            ↓
        Payment Activity


**2. Service:** 
- A Service performs work in the background without requiring a user interface.
- The user may not be directly interacting with the Service.

- **Real-life example:**
    - Think about playing music or Tracking a user's location when appropriate.
    - You open a music application and start a song:

            Music App
                ↓
            Start Music
                ↓
            Service
                ↓
            Music continues playing

    - Even if you leave the music application's screen, the music can continue playing.

- **Practical use cases**

    - Playing music
    - Processing ongoing work
    - Tracking a user's location when appropriate
    - Performing certain background operations
    - Maintaining an ongoing task


**3. Broadcast Receiver**

- A Broadcast Receiver **listens for specific events** or **broadcasts** and reacts when those events occur.
- An event can be generated by the Android system or by an application.

- **Real-life example**  
    - Think about a doorbell.

            Someone presses doorbell
                    ↓
            Bell receives signal
                    ↓
            Bell rings

    - Similarly:

            Android Event
                ↓
            Broadcast Receiver
                ↓
            Application performs action

- **Practical example**

    - Suppose an application wants to perform some action when the device finishes booting:

            Phone Starts
                ↓
            BOOT_COMPLETED Event
                ↓
            Broadcast Receiver
                ↓
            Application responds

- **Examples of events**
    - Device boot completion
    - Connectivity-related changes
    - Battery-related events
    - Application-defined broadcasts


**4. Content Provider:**

- A Content Provider is an Android component used to store and share data between applications in a controlled way.
- A Content Provider can allow applications to:
    - Read data
    - Add data
    - Update data
    - Delete data

- **🧠 Simple Example**
    - Imagine you have a Contacts app on your phone.
    - Your contacts are stored somewhere in the phone. Another app, such as a messaging app, may need to access your contacts.
    - Instead of allowing the messaging app to directly access the contacts database, Android provides a **Content Provider**.

                  Contacts Data
                        ↑
                        │
                  Content Provider
                        ↑
                  ┌─────┴─────────┐─────────────┐
                  │               │             |
              Contacts App   Messaging App   WhatsApp


- **Real-life example**

    - Think of a bank counter:

            You
            ↓
            Bank Counter
            ↓
            Bank Database

    - You don't directly enter the bank's database. You make a request through the counter.  
    Similarly:

            Application
            ↓
            Content Provider
            ↓
            Data

- **Practical use cases**

    - An application needs to access contacts.
    - Applications need controlled access to shared data.
    - Data needs to be shared between applications.



## Ques 4. Describe the complete Activity Lifecycle with the help of a neat diagram. Explain the purpose of each lifecycle callback method and discuss its significance in Android application development.



