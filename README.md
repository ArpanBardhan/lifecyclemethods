# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: ARPAN BARDHAN
Registeration Number : 212222040013
*/
```
activity_main.xml
```XML
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:textSize="24sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
AndroidManifest.xml
```XML
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@drawable/ic_launcher_foreground"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.MobileAppdemo"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```
MainActivity.java
```JAVA
package com.example.mobileappdemo;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(),"onCreate Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart(){
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(),"onRestart Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(),"onStop Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(),"onDestroy Called",Toast.LENGTH_LONG);
        toast.show();
    }
}
```

## OUTPUT
![Screenshot (427)](https://github.com/ArpanBardhan/lifecyclemethods/assets/119405037/8be9f6da-41a5-41b6-97e1-045e206c1c4c)
![Screenshot (428)](https://github.com/ArpanBardhan/lifecyclemethods/assets/119405037/0af4f9e3-a96e-4b29-8284-a8d3acc7b247)
![Screenshot (429)](https://github.com/ArpanBardhan/lifecyclemethods/assets/119405037/7d3627ff-4415-488b-ab22-8d1f504b1603)
![Screenshot (430)](https://github.com/ArpanBardhan/lifecyclemethods/assets/119405037/870554d2-81e8-4eec-adf1-7c996b92dd9e)
![Screenshot (432)](https://github.com/ArpanBardhan/lifecyclemethods/assets/119405037/b7553063-5a99-4228-9cef-a702a9661a5f)
![Screenshot (433)](https://github.com/ArpanBardhan/lifecyclemethods/assets/119405037/38c053e4-e0fc-44b9-9894-465e171d1de4)




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
