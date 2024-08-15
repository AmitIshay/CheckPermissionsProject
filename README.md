## Check Permissions App


# Overview


The Check Permissions App is an Android application that allows users to view, request, and check the status of various permissions required by the app.


permissions along with their status (granted or not) and allows users to request the necessary permissions.


# Features


* List of Permissions: The app displays a list of all the permissions that are required by the app, including INTERNET, CALL_PHONE, VIBRATION, RECORD_AUDIO, LOCATION, SMS, CONTACTS, CAMERA, CALENDAR, SENSORS, and BLUETOOTH.


* Permission Status: The app visually indicates whether each permission is granted or not using a colored card. Green indicates that the permission is granted, while red indicates it is not.


* Request Permissions: Users can request permissions by tapping on any permission that is not granted. The app will prompt the user to allow or deny the permission.


* Permission Change Listener: The app automatically updates the permission status whenever a permission is granted or revoked.


## How It Works


# Main Components


* MainActivity: The main activity of the app where the permissions list is displayed. It handles the registration and unregistration of the permission change listener and manages the permissions request process.


* PermissionsModel: A data model representing each permission with its name, associated image, and status (granted or not).


* Adapter: The RecyclerView adapter that binds the PermissionsModel data to the RecyclerView items.


* RecyclerViewInterface: An interface to handle item click events in the RecyclerView.


# Permission Management


The app uses the PermissionsManager class from the permissionslib library to handle permission-related tasks, such as checking if permissions are granted, requesting permissions, and notifying the app when permission statuses change.
