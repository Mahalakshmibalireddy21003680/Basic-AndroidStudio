# Ex.No:8 Build a program to show five checkboxes and toast selected checkboxes.


## AIM:

To create a list using checkbox to display selected checkbox item using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min.required Artic Fox)

## ALGORITHM:



## PROGRAM:
```
/*
Program to display check list item”.
Developed by:Balireddy Mahalakshmi
Registeration Number :212221240008
*/
```
### MainActivity.java:
~~~~
package com.example.exp8;



import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

import android.view.View;
import android.widget.CheckBox;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    private CheckBox chkAndroid, chkJava, chkPhp, chkCpp, chkC;

    @Override
    public void onCreate(Bundle savedInstanceState) {

        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        chkAndroid = findViewById(R.id.chkAndroid);
        chkJava = findViewById(R.id.chkJava);
        chkPhp = findViewById(R.id.chkPhp);
        chkCpp = findViewById(R.id.chkCpp);
        chkC = findViewById(R.id.chkC);
    }

    public void showSelected(View view) {

        String selected = "You selected: \n";

        if(chkAndroid.isChecked())
            selected += "Android";

        if(chkJava.isChecked())
            selected += "\nJava";

        if(chkPhp.isChecked())
            selected += "\nPHP";

        if(chkCpp.isChecked())
            selected += "\nCPP";

        if(chkC.isChecked())
            selected += "\nC";

        Toast.makeText(MainActivity.this, selected, Toast.LENGTH_SHORT).show();
    }
}
~~~~
### activity_main.xml:
~~~~
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="fill_parent"
    android:layout_height="fill_parent"
    android:orientation="vertical"
    android:padding="20dp">

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:text="Select Your favourite Programming language"
        style="@style/TextAppearance.AppCompat.Large"
        android:layout_margin="10dp"
        android:textStyle="bold"/>

    <CheckBox
        android:id="@+id/chkAndroid"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Android"
        style="@style/TextAppearance.AppCompat.Headline"/>

    <CheckBox
        android:id="@+id/chkJava"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Java"
        style="@style/TextAppearance.AppCompat.Headline"/>

    <CheckBox
        android:id="@+id/chkPhp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="PHP"
        style="@style/TextAppearance.AppCompat.Headline"/>

    <CheckBox
        android:id="@+id/chkCpp"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="CPP"
        style="@style/TextAppearance.AppCompat.Headline"/>

    <CheckBox
        android:id="@+id/chkC"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="C"
        style="@style/TextAppearance.AppCompat.Headline"/>

    <Button android:id="@+id/btnDisplay"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Display"
        android:layout_marginTop="20dp"
        android:onClick="showSelected"/>

</LinearLayout>
~~~~~~
## OUTPUT:

![a](https://user-images.githubusercontent.com/93427286/200482068-453a7da8-f20b-4140-8eb7-62593732dfb7.jpg)
![b](https://user-images.githubusercontent.com/93427286/200482103-02fe3a2d-341c-4c5c-bfe0-0a4fb5289c46.jpg)
![c](https://user-images.githubusercontent.com/93427286/200482179-42a5d204-5201-4d56-8ab1-63c942b89662.jpg)
![d](https://user-images.githubusercontent.com/93427286/200482186-7d98ae9e-3fc6-444d-8e4f-e017974cc086.jpg)


## RESULT
Thus a Simple Android Application create a list using checkbox to display selected checkbox using Android Studio is developed and executed successfully.
