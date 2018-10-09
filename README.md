# react-navigation-deprecated-tab-navigator
TabBar at bottom on Android.

What is this project for?

Here's the backstory.

React Native Router Flux uses React Navigation package as a dependency and uses its component for creating navigation based components like navbar, drawer, bottom bar etc.
Starting v4, RNRF uses v2 of React Navigation.
v2 of React Navigation removed the Bottom Tab Bar features like swipe support and animations for some reasons whatsoever.

Now a solution to that is to use the legacy prop in <Tabs> component of RNRF but the behavious is that on iOS the tabbar shows on bottom and on Android it shows on top.
Once the legacy flag is set to to true, it does not take into consideration the value of tabBarPosition.

Luckily, RN(avigation) guys created a seperate project called react-navigation-deprecated-tab-navigator which brings back features like swipe support and animations when using v2 of RN.

But again, it shows tabbar on top in android and on bottom of screen on iOS which is inconsistent behavior.

So, I hardcoded the value of position for android to top.

TLDR: Bottom Tab Navigation Bar for android when using v4 RNRF and v2 RN.
