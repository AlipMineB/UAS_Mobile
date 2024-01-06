# UAS_Mobile
Nama          : Muhammad Alif .F
NIM           : 312210163
Kelas         : TI.22.A1
Mata Kuliah   : Pemrograman Monile 1
Dosen         : Donny Maulana, S.Kom., M.M.S.I.

# 1. Hello World
# String
 <string name="hello_worldd">Hello World!</string>

 # Java
 # HelloActivity.java
 package com.alipapps;

import android.os.Bundle;
import androidx.appcompat.app.AppCompatActivity;

public class HelloActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_hello);

    }
}

# Layout
# activity_hello.xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".HelloActivity">

    <TextView
        android:id="@+id/Texthello"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="courier"
        android:gravity="center"
        android:text="@string/hello_worldd"
        android:textColor="@color/white"
        android:textSize="15pt"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.500"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.257"
        tools:ignore="TextSizeCheck" />

</androidx.constraintlayout.widget.ConstraintLayout>
