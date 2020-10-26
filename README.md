# Build a simple React-Native photo app in 30 minutes

## Introduction

I was recently working on a React-Native project where we needed to give the user the ability to include photos from either their library or take a photo with their device camera. I wanted to build the project with the Expo "Managed workflow" so I could test it wirelessly on my device. I found ImagePicker (expo-image-picker) but until I started looking at the API reference, I didn't realize it also allow you to use the camera in addition to picking an existing photo from the device library.

This tutorial will show you how to build a simple Expo Managed React-Native photo app. The app simply allows you to select a photo from your library or take a photo with the camera and then displays it on the main screen. It is intended to be a boilerplate to get you started building your own photo app.

To get started, we will need a React-Native project. You can follow these instructions to set up a project or create a React-Native project using Expo or your preferred method.

## Prerequisites

-   Some comfort using command-line tools.

-   Install the latest version of NodeJS on your development machine. Your development machine can be Windows, Linux, or macOS even if you are developing for an iOS device!

## Create your React Native project using Expo

### Why Expo?

Expo is a great way to get a React-Native project running on your mobile device without hard-wiring to your develop machine. Previously, if you were building a mobile application, you would have to connect a Lightning or USB cable between your development machine and your mobile device to test out your app on your mobile device. If you were developing an iOS app you would have to use a Mac running Xcode to get your app on your device. This is pretty silly considering both devices have a network connection. Expo offers an alternative.

### How does Expo work?

Expo has two parts:

-   **expo-cli** is a command-line, npm-installed, network service that runs on your development machine. It integrates with your project and makes it accessible by your mobile device on your local network.
    As long as your development machine is on the same network as your mobile device
-   **Expo Client** is an app available on iOS and Android.

Let's get start:

-   At a command-line use npm to install **expo-cli** on your machine. Use the "-g" switch to make it global.

    `npm install -g expo-cli`

-   Use the Expo to initialize a new React-Native project with Expo integration. Replace "MyProject" with the name of your project.

    `expo init MyProject`

-   Now start your project and make it available on your network to the Expo mobile app:

    `npm start`

## Add expo-image-picker to your project

-   Use npm to install ImagePicker:

    `npm install expo-image-picker`
