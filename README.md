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
Developed by: Sanjit A
Registeration Number : 212224220087
*/
```

## MainActivity.java:
```
package com.example.sampleactivity;

import android.os.Bundle;
import android.widget.Toast;


import androidx.appcompat.app.AppCompatActivity;


public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast= Toast.makeText(getApplicationContext(),"onCreate Called", Toast.LENGTH_SHORT);
        toast.show();
    }
    @Override
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnStart called", Toast.LENGTH_LONG);
        toast.show();
    }

    @Override
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "OnPause called", Toast.LENGTH_SHORT);
        toast.show();
    }

    @Override
    protected void onResume() {
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "OnResume called", Toast.LENGTH_SHORT);
        toast.show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnRestart called", Toast.LENGTH_SHORT);
        toast.show();
    }

    @Override
    protected void onStop() {
        super.onStop();

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onStop called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }
    @Override
    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "OnDestroy called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```

## activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="144dp"
        android:text="LifeCycleActivity"
        android:textSize="28sp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Welcome to Android Studio"
        android:textSize="26sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.494"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView"
        app:layout_constraintVertical_bias="0.584" />
</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT:-

## OnCreate():
<img width="1917" height="1136" alt="image" src="https://github.com/user-attachments/assets/db89e6ff-0d85-4a5b-adfa-ec99525512dc" />

## OnStart():
<img width="1917" height="1133" alt="image" src="https://github.com/user-attachments/assets/4b0dbba0-b0cb-40fe-8534-f927883028a3" />

## OnRestart():
<img width="1917" height="1135" alt="image" src="https://github.com/user-attachments/assets/6802e839-1ee1-4a76-a48f-cfac32d03b1f" />

## OnPause():
<img width="1917" height="1142" alt="image" src="https://github.com/user-attachments/assets/73d1d8c4-750c-4c23-bab0-3f937391a631" />

## OnResume():
<img width="1911" height="1137" alt="image" src="https://github.com/user-attachments/assets/433266a7-e887-4300-9462-c9a331cdf52f" />



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
