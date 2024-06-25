# ReduxRefresher

ReduxRefresher

npm install react-redux
npm install @reduxjs/toolkit

can use functions for firebase backend - but we dont use this in this project using realtime database

Using Firebase as a Backend

In the next lecture, we'll use a third-party service called [Firebase](https://firebase.google.com/) as a dummy backend.

**You can get started with Firebase for free** - all you need is a Google account.

Then, once logged in with Google, you can create a **new project** with the default settings. Though you can disable "Google Analytics".

Thereafter, click **"Build"** and select **"Realtime Database"** and click **"Create Database"**.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2023-11-28_15-36-11-7be2236b66f209ec0d0ac5df856e2cdc.jpg)

The region doesn't matter but make sure to create the database in **"Test mode"**!

This will create the database with a connected REST API that we'll use throughout this section.

You can then **use the URL displayed on the screen** in your React code to send requests to that database. That's what we'll do throughout the next lectures.

![](https://img-c.udemycdn.com/redactor/raw/article_lecture/2023-11-28_15-36-11-b77f0ce79a4a19a041735b1b61b8c980.jpg)
https://reactcart-49bf0-default-rtdb.firebaseio.com/

A Problem with useEffect()
We face one problem when using useEffect the way we currently do it: It will execute when our app starts.

Why is this an issue?

It's a problem because this will send the initial (i.e. empty) cart to our backend and overwrite any data stored there.

We'll fix this over the next lectures, I just wanted to point it out here!

https://reactcart-49bf0-default-rtdb.firebaseio.com/cart.json

Using Thunks - delayed actions

sideeffects and async
