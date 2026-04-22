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

Program to print the text “Hello World”.

Developed by: Subash M
Registeration Number : 212224220109

mainactivity.java
```
package com.example.myapplication;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        setContentView(R.layout.activity_main);
        Toast toast= Toast.makeText(getApplicationContext(),"OnCreated Executed",Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onStart(){
        super.onStart();
        Toast toast= Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast= Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast= Toast.makeText(getApplicationContext(),"onPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast= Toast.makeText(getApplicationContext(),"onStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast= Toast.makeText(getApplicationContext(),"onRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast= Toast.makeText(getApplicationContext(),"onDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}
```
activity_main.xml

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
        android:id="@+id/textView2"
        style="@android:style/Widget.TextView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:shadowColor="@color/black"
        android:text="Hello World!"
        android:textColor="@color/design_default_color_primary_variant"
        android:textSize="34sp"
        android:textStyle="bold|italic"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.501"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.473" />

    <TextView
        android:id="@+id/textView"
        style="@style/Widget.AppCompat.TextView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Lifecycle Methods"
        android:textColor="@color/design_default_color_error"
        android:textColorHint="@color/design_default_color_error"
        android:textColorLink="@color/design_default_color_error"
        android:textSize="34sp"
        android:textStyle="bold|italic"
        app:layout_constraintBottom_toTopOf="@+id/textView2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

```


## OUTPUT

# 1.Oncreated execution 

<img width="1919" height="1079" alt="1" src="https://github.com/user-attachments/assets/0ba67dee-c3b9-4397-8dc2-dac5e83c4450" />

# 2.Onstart execution 

<img width="1919" height="1079" alt="2" src="https://github.com/user-attachments/assets/b6a8660b-777c-43c4-aeec-9ae86ad1225d" />

# 3.Onresume execution 

<img width="1916" height="1078" alt="3" src="https://github.com/user-attachments/assets/ee463eb5-7166-4ec1-8ee2-f5f6c515cdd4" />

# 4.Onrestart execution 

<img width="1919" height="1079" alt="4" src="https://github.com/user-attachments/assets/c9297476-abea-47a1-b7d7-a050dea5a430" />

# 5.Onpause execution 

<img width="1919" height="1079" alt="5" src="https://github.com/user-attachments/assets/5d7dd929-7146-4c25-934e-ef64d10e38b6" />



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
