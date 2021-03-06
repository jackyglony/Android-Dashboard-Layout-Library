## Android Dashboard Layout Library

Use this library to create your app dashboard easily - without worrying about `GridLayout`, `Adapter` and such other stuffs. This library is based on the [source code](https://code.google.com/p/iosched/) of Google IO 2013 app.

### Screenshot
![Screenshot](https://raw.githubusercontent.com/rafi-kamal/Android-Dashboard-Layout-Library/master/screenshot.png)


### Compatibility

Supports Android 2.2+ (API level 8).

### Usage

+ Import the project in Eclipse `(File > Import > Existing Projects into Workspace)`
+ Add this library as a reference in your project `(Properties > Android > (Library) Add)`
+ You don't need to change anything in your Activity. Just change the root of the xml layout file to `cubi.rafi.DashboardLayout` instead of `LinearLayout`, `RelativeLayout` etc.
+ It is recommended to use `style/DashboardButton` as the style of your Buttons.

### Example 

```xml
<cubi.rafi.DashboardLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="fill_parent"
    android:layout_height="fill_parent" >

    <Button android:id="@+id/dashboard_user"
        style="@style/DashboardButton"
        android:text="My Profile"
        android:drawableTop="@drawable/dashboard_user" />

    <Button android:id="@+id/dashboard_emergency_contact"
        style="@style/DashboardButton"
        android:text="Emergency Contact"
        android:drawableTop="@drawable/dashboard_call" />

    <Button android:id="@+id/dashboard_new_accident"
        style="@style/DashboardButton"
        android:text="New Accident"
        android:drawableTop="@drawable/dashboard_add" />

    <Button android:id="@+id/dashboard_send_case"
        style="@style/DashboardButton"
        android:text="Send Case"
        android:drawableTop="@drawable/dashboard_message" />

    <Button android:id="@+id/dashboard_record"
        style="@style/DashboardButton"
        android:text="Record"
        android:drawableTop="@drawable/dashboard_record" />

    <Button android:id="@+id/dashboard_tow_truck"
        style="@style/DashboardButton"
        android:text="Tow Truck"
        android:drawableTop="@drawable/dashboard_truck" />
 
</cubi.rafi.DashboardLayout>
```
