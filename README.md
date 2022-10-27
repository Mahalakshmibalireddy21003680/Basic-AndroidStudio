# Basic-AndroidStudio
```
Developed By: B.Mahalakshmi
Registered Number: 212221240008
```

### MainActivity.java:
```
package com.example.lifecycle;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);




        Toast toast = Toast.makeText(getApplicationContext(), "OnCreate Executed", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}
```

### activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="HelloWorld!"
        android:layout_centerVertical="true"
        android:layout_centerHorizontal="true"
        android:textSize="20sp"
        android:textColor="@color/black"

        />
</RelativeLayout>
```

### Output:
![li1](https://user-images.githubusercontent.com/93427286/198373248-bed63ce0-4cbd-41c0-ab74-49253f948d3d.jpg)
![li2](https://user-images.githubusercontent.com/93427286/198373256-53e91bd9-3ad6-4bd1-860c-85105fa6d959.jpg)
![li3](https://user-images.githubusercontent.com/93427286/198373260-cc21387c-9e84-4ce0-91fc-cf52dd66ed11.jpg)
![li4](https://user-images.githubusercontent.com/93427286/198373268-6706481c-0b38-4e99-8d2e-116b4a6068e1.jpg)
![li5](https://user-images.githubusercontent.com/93427286/198373269-07b4b0c7-097d-4341-bfcf-7290801dfc18.jpg)
![li6](https://user-images.githubusercontent.com/93427286/198373274-6bc7dc07-c4ad-4a97-a64c-8c7ed7be8289.jpg)

### Result:
Therefore a program is return to develop a program to detect the various life cycles of an activity. The program is successfully executed.
