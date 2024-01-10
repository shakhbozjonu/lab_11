# Lab 11

This Flutter application demonstrates Firebase integration for authentication and Firestore database usage for user registration and data storage.

## Overview

The application consists of three screens:
- **Login Screen**: Allows users to sign in using Firebase authentication or navigate to the registration screen.
- **Registration Screen**: Enables users to create a new account by providing a username, password, and email. The user data is stored in Firestore.
- **Main Page**: Displays the user's email fetched from Firestore after successful login or registration.

## Implementation Details
- login: email@example.com
- password: SuperSecretPassword!

### Firebase Integration

The code integrates Firebase into the Flutter application for authentication and Firestore database operations.

#### Authentication
- Uses Firebase's `signInAnonymously` method for anonymous authentication.
- Implements the sign-in functionality by checking user credentials and navigating to the main page upon successful authentication.

#### Registration
- Uses Firebase's `createUserWithEmailAndPassword` method to create a new user account with an email and password.
- Stores user information (username and email) in Firestore under the 'users' collection.

#### Main Page
- Retrieves the user's email from Firestore based on the authenticated user's UID.
- Displays the user's email on the main page after successful authentication or registration.

