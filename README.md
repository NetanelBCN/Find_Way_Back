
# Decompiled Game Project


## Overview

This project involves decompiling an Android game using Java and Android Studio, making several modifications to enhance its functionality and user experience. The game features a menu screen where users enter their ID, and a game screen with directional arrows that players press according to their ID digits.

# Modifications

## 1. Fixed URL in strings file: Corrected the URL to ensure the game points to the correct web resource.

## 2. Simplified integer parsing in array population code:
Previous code: iArr[i] = Integer.valueOf(String.valueOf(id.charAt(i))).intValue() % 4;
Updated code: iArr[i] = Integer.parseInt(String.valueOf(id.charAt(i))) % 4;

This change simplifies the conversion of id.charAt(i) to an integer and then takes the modulus operation.

## 3. Updated toast message duration:

### From: 

Toast.makeText(this, "Survived in " + state, 1).show();
Toast.makeText(this, "You Failed ", 1).show();

### To:

Toast.makeText(this, "Survived in " + state, Toast.LENGTH_LONG).show();
Toast.makeText(this, "You Failed ", Toast.LENGTH_LONG).show();

## 4. Added internet permission to manifest:

<uses-permission android:name="android.permission.INTERNET" />


# Game Description

Menu Screen: Users enter their ID and press the start button.
Game Screen: There are four arrows (up, down, left, right).
The program takes each digit from the user ID and performs a modulus 4 operation.
The results determine the arrow presses:

0: Left

1: Right

2: Up

3: Down



## Features

- #### User Account Creation
  Users can easily create accounts using either their    phone numbers or Gmail accounts.


- #### Child Profiles:
  Parents or guardians can add new kids to the application, each with their own profile.
- #### Immunization Records:
  Keep track of each child's immunization history, ensuring they stay up-to-date with vaccinations.

- #### Event Tracking:
  Maintain a list of events for each child, helping users manage their schedules effectively.

- #### Photo Gallery:
  Store precious memories by adding photos to each child's profile.

- #### Firebase Integration:
  All data, including immunization records, event lists, and photos, are securely stored in Firebase Realtime Database and Firebase Storage, ensuring reliability and accessibility.





## Watch Me!




https://github.com/NetanelBCN/Find_Way_Back/assets/134021385/df6cb328-8d85-4c21-ae86-ec427136441d






