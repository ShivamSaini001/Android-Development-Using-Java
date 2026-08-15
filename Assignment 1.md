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

**1. Applications Layer:** This is the **top layer** of Android architecture. It contains applications that users directly interact with.  
Applications can be **pre-installed system applications** or applications installed by the user.

The Applications layer provides the actual functionality that the user needs.  
*For example:*  User ➡ Click on Camera App ➡ Camera Application open  

The camera application doesn't directly control the camera hardware. It uses Android's lower layers to access it.


### 2. Application Framework Layer

This layer provides **ready-made services** to applications.  
For example, suppose your app wants to:
- Open a camera
- Show a notification
- Find your location
- Create a window
- Manage an activity

Instead of building everything from scratch, the app asks Android's Application Framework.
For example:
```C
    Camera App
        ↓
    Camera-related Android APIs/services
        ↓
    Camera Hardware
```


### 3. Android Runtime + Native Libraries





