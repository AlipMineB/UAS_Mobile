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

# 2. Movie (Ice Cold)
# String
<string name="article_tittle">Kasus Sianida</string>
<string name="article_subtitle">ICE COLD</string>
<string name="article_text"> Film dokumenter Ice Cold: Murder, Coffee and Jessica Wongso memaparkan pertanyaan tak terjawab tentang persidangan yang dilalui Jessica Wongso. Dengan menyajikan perspektif baru, film ini hadir bertahun-tahun setelah kematian sahabat Jessica, Wayan Mirna Salihin.

    Film ini menggambarkan bagaimana Jessica yang mengajak teman-temannya, termasuk Mirna, untuk bertemu setelah sekian lama tak berjumpa. Pertemuan di salah satu kafe di mal ibu kota tersebut pun berlangsung lancar, sebelum akhirnya Mirna pingsan sesaat setelah meminum kopi yang sebelumnya dipesan Jessica.
    Dokumenter ini turut menyajikan rekaman CCTV pada waktu kejadian, berbagai footage berita saat persidangan berlangsung, hingga wawancara eksklusif dengan beberapa sumber, termasuk Jessica Wongso.

    Persidangan atas dugaan pembunuhan Mirna Salihin digelar lima bulan setelah kematiannya. Sidang tersebut melalui 32 kali persidangan dengan menghadirkan puluhan saksi di pengadilan. Hasilnya, Jessica Wongso divonis bersalah atas kematian Mirna dan dijatuhi hukuman 20 tahun penjara.
    Kasus yang berjalan cukup lama tersebut menyita banyak perhatian dari masyarakat Indonesia. Musababnya, banyak misteri tak terjawab selama rangkaian persidangan yang panjang tersebut. Salah satunya adalah mengenai akses untuk mendapatkan bubuk sianida yang tidak bisa didapatkan oleh orang sembarangan. Selain itu, motif Jessica di balik pembunuhan tersebut pun belum menemukan jawabannya.

    Film dokumenter buatan Netflix ini menyoroti rangkaian persidangan yang saat itu menjadi sidang pertama yang disiarkan secara langsung di berbagai stasiun televisi Indonesia. Selain itu, kasus ini juga diliput secara intens oleh media massa, baik nasional maupun internasional.Tak hanya itu, pihak rumah produksi Beach House Pictures juga berhasil mendapatkan akses untuk mewawancarai Jessica Wongso secara langsung dari balik tahanan. Dalam video trailer yang diluncurkannya, ditampilkan juga sejumlah wawancara eksklusif yang dilakukan dengan beberapa narasumber. Mulai dari ayah dan saudara kembar  Mirna Salihin, pengacara Jessica Wongso, jurnalis yang mendalami kasus tersebut, hingga bagaimana saat itu kasus ini begitu ramai diberitakan oleh media massa Indonesia dan internasional.</string>

# Java
# MovieActivity.java
package com.alipapps;

import android.os.Bundle;

import androidx.appcompat.app.AppCompatActivity;

public class SianidaActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_sianida);
    }
}

# Layout
# activity_movie.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".SianidaActivity">

    <ScrollView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/article_heading">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:orientation="vertical">

            <TextView
                android:id="@+id/article_subheading"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:padding="10dp"
                android:text="@string/article_subtitle"
                android:textAppearance="@android:style/TextAppearance.DeviceDefault" />

            <TextView
                android:id="@+id/article"
                android:layout_width="match_parent"
                android:layout_height="643dp"
                android:autoLink="web"
                android:lineSpacingExtra="@dimen/line_spacing"
                android:padding="10dp"
                android:justificationMode="inter_word"
                android:text="@string/article_text" />
        </LinearLayout>
    </ScrollView>
</RelativeLayout>
# 3. Toast Fibonaci
# String
<string name="button_label_toast">Toast</string>
<string name="button_label_count">Count</string>
<string name="count_initial_value">1</string>
<string name="toast_message">Hello Toast!</string>

# Color
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="black">#FF000000</color>
    <color name="white">#FFFFFFFF</color>
    <color name="blue">#3700B3</color>
    <color name="pink">#FFC0CB</color>
    <color name="colorPrimary">#3F5185</color>
    <color name="colorPrimaryDark">#303F9F</color>
    <color name="colorAccent">#FF4081</color>
    <color name="birumuda">#ABCBFA</color>
    <color name="salem">#F8C6E6</color>
    <color name ="purple">#E3A2ED</color>
    <color name="hijau">#92A676</color>
    <color name="biru">#8FC2EA</color>
    <color name="hijaumuda">#C2E69C</color>
    <color name="kuning">#FFEB3B</color>
    <color name="orange">#FF9800</color>
    <color name="cream">#E6C18A</color>
    <color name="pink_terang">#ffb6c1</color>
    <color name="koral">#f08080</color>
</resources>

# Java
# ToastActivity.java
package com.alipapps;

import android.app.AlertDialog;
import android.content.DialogInterface;
import android.graphics.Color;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;


public class ToastActivity extends AppCompatActivity {
    private TextView show_count;
    private int count = 1;
    private long fibNMinus1 = 1;
    private long fibNMinus2 = 1;
    private int limit = -1; // Inisialisasi limit dengan nilai default

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_toast);

        show_count = findViewById(R.id.show_count);
    }

    public void countUp(View view) {
        if (count == 0) {
            show_count.setText("0");
        }
        else if (count == 1) {
            show_count.setText("1");
        }
        else {
            if (limit != -1 && count > limit) {
                // Jika count melebihi limit, atur ulang perhitungan
                count = 0;
                fibNMinus1 = 1;
                fibNMinus2 = 0;
                show_count.setText(getString(R.string.count_initial_value));
            }
            else {
                long fibCurrent = fibNMinus1 + fibNMinus2;
                fibNMinus2 = fibNMinus1;
                fibNMinus1 = fibCurrent;

                //Mengatur warna teks berdasarkan angka Fibonacci
                int colorResId = R.color.orange; // Warna Default
                switch (count % 11) {
                    case 1:
                        colorResId = R.color.pink_terang; // Warna Orange
                        break;
                    case 2:
                        colorResId = R.color.hijaumuda; // Warna Hijau Muda
                        break;
                    case 3:
                        colorResId = R.color.purple; // Warna Ungu
                        break;
                    case 4:
                        colorResId = R.color.salem; // Warna Salem
                        break;
                    case 5:
                        colorResId = R.color.birumuda; // Warna Biru Muda
                        break;
                    case 6 :
                        colorResId = R.color.koral; // Warna Kuning
                        break;
                    case 7:
                        colorResId = R.color.hijau; // Warna Hijau
                        break;
                    case 8:
                        colorResId = R.color.cream; // Warna Cream
                        break;
                    case 9:
                        colorResId = R.color.pink; // Warna Pink
                        break;
                    case 10:
                        colorResId = R.color.biru; // Warna Biru
                        break;
                    case 11:
                        colorResId = R.color.colorAccent; // Warna Pink Tua
                        break;
                }
                show_count.setTextColor(getResources().getColor(colorResId));
                show_count.setText(String.valueOf(fibCurrent));
            }
        }

        count++;
    }

    public void restart(View view) {
        count = 1;
        fibNMinus1 = 1;
        fibNMinus2 = 0;
        show_count.setText(getString(R.string.count_initial_value));
    }

    public void setLimit(View view) {
        // Create and display a dialog to set the limit
        AlertDialog.Builder builder = new AlertDialog.Builder(this);
        builder.setTitle("Set Limit");

        final EditText input = new EditText(this);
        input.setInputType(android.text.InputType.TYPE_CLASS_NUMBER);
        builder.setView(input);

        builder.setPositiveButton("OK", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                // Get the limit from the input and set it for calculations
                String limitStr = input.getText().toString();
                limit = Integer.parseInt(limitStr);
            }
        });

        builder.setNegativeButton("Cancel", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                dialog.cancel();
            }
        });

        builder.show();
    }
}

# Layout
# activity_movie.xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:ignore="ExtraText"
    tools:context=".ToastActivity">

    <Button
        android:id="@+id/button_limit"
        android:layout_width="440dp"
        android:layout_height="60dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:background="@color/colorPrimary"
        android:onClick="setLimit"
        android:text="Masukkan Angka Limit"
        android:textColor="@android:color/white"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.454"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:ignore="UsingOnClickInXml,VisualLintButtonSize" />

    <Button
        android:id="@+id/button_count"
        android:layout_width="180dp"
        android:layout_height="80dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:layout_marginStart="10dp"
        android:layout_marginBottom="10dp"
        android:background="@color/colorPrimary"
        android:onClick="countUp"
        android:text="Count"
        android:textColor="@android:color/white"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button_restart"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml,VisualLintButtonSize" />

    <Button
        android:id="@+id/button_restart"
        android:layout_width="180dp"
        android:layout_height="80dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentEnd="true"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="10dp"
        android:layout_marginBottom="10dp"
        android:background="@color/colorPrimary"
        android:onClick="restart"
        android:text="Restart"
        android:textColor="@android:color/white"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml" />

    <TextView
        android:id="@+id/show_count"
        android:layout_width="400dp"
        android:layout_height="550dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="10dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="10dp"
        android:background="@drawable/bg_count"
        android:gravity="center_vertical"
        android:text="1"
        android:textAlignment="center"
        android:textColor="@color/colorPrimary"
        android:textSize="160sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@id/button_count"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/button_limit"
        app:layout_constraintVertical_bias="0.0"
        tools:ignore="RtlCompat" />

</androidx.constraintlayout.widget.ConstraintLayout>

# 4. Two Activity Send and Reply Message
# String
 <string name="button_main">Send</string>
    <string name="editText_main">Enter Your Message Here</string>
    <string name="text_header">Messege Received</string>
    <string name="button_second">Reply</string>
    <string name="editText_second">Enter Your Reply Here</string>
    <string name="text_header_reply">Reply Received</string>

# Java (send)
# SendActivity.java
package com.alipapps;

import android.content.Intent;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

import androidx.appcompat.app.AppCompatActivity;

public class SendActivity extends AppCompatActivity {

    public static final String EXTRA_REPLY ="com.example.android.Reply.extra.REPLY";

    private EditText mReply;

    @Override
    protected void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_send);

        mReply = findViewById(R.id.editText_second);

        Intent intent = getIntent();
        String message = intent.getStringExtra(ReplyActivity.EXTRA_MESSAGE);

        TextView textView = findViewById(R.id.text_message);
        textView.setText(message);
    }
    public void returnReply(View view){
        String reply = mReply.getText().toString();
        Intent replyIntent = new Intent();
        setResult(RESULT_OK, replyIntent);
        finish();
    }
}

# Layout (send)
# activity_send.xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    tools:context=".SendActivity">

    <TextView
        android:id="@+id/text_header"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="16dp"
        android:text="@string/text_header"
        android:textAppearance="@style/TextAppearance.AppCompat.Medium"
        android:textStyle="bold"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/text_message"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="8dp"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/text_header" />

    <Button
        android:id="@+id/button_second"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="16dp"
        android:layout_marginRight="16dp"
        android:text="@string/button_second"
        android:onClick="returnReply"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        tools:ignore="UsingOnClickInXml" />

    <EditText
        android:id="@+id/editText_second"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="16dp"
        android:ems="10"
        android:hint="@string/editText_second"
        android:inputType="textLongMessage"
        android:minHeight="48dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button_second"
        app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>

# Java (reply)
# ReplyActivity.java
package com.alipapps;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.util.Log;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

public class ReplyActivity extends AppCompatActivity {

    private static final String LOG_TAG = ReplyActivity.class.getSimpleName();

    public static final String EXTRA_MESSAGE = "com.example.android.SendActivity.extra.MESSAGE";

    public static final int TEXT_REQUEST = 1;

    private EditText mMessageEditText;

    private TextView mReplyHeadTextView;

    private TextView mReplyTextView;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_reply);

        mMessageEditText = findViewById(R.id.editText_main);
        mReplyHeadTextView = findViewById(R.id.text_header_reply);
        mReplyTextView = findViewById(R.id.text_message_reply);
    }

    public void LaunchSecondActivity(View view) {
        Log.d(LOG_TAG, "Button clicked!");
        Intent intent = new Intent(this, SendActivity.class);
        String message = mMessageEditText.getText().toString();
        intent.putExtra(EXTRA_MESSAGE, message);
        startActivityForResult(intent, TEXT_REQUEST);
    }

    @Override
    public void onActivityResult(int requestCode, int resultCode, Intent data) {
        super.onActivityResult(requestCode, resultCode, data);

        if (requestCode == TEXT_REQUEST) {
            if (resultCode == RESULT_OK) {
                String reply = data.getStringExtra(SendActivity.EXTRA_REPLY);

                mReplyHeadTextView.setVisibility(View.VISIBLE);
                mReplyTextView.setText(reply);
                mReplyTextView.setVisibility(View.VISIBLE);
            }
        }
    }
}

# Layout (reply)
# activity_reply.xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    tools:context=".ReplyActivity">

    <TextView
        android:id="@+id/text_header_reply"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="16dp"
        android:text="@string/text_header_reply"
        android:textAppearance="@style/TextAppearance.AppCompat.Medium"
        android:textStyle="bold"
        android:visibility="invisible"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>

    <TextView
        android:id="@+id/text_message_reply"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="8dp"
        android:visibility="invisible"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/text_header_reply" />

    <Button
        android:id="@+id/button_main"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="16dp"
        android:layout_marginRight="16dp"
        android:text="@string/button_main"
        android:onClick="LaunchSecondActivity"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        tools:ignore="UsingOnClickInXml"/>

    <EditText
        android:id="@+id/editText_main"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="16dp"
        android:ems="10"
        android:hint="@string/editText_main"
        android:inputType="textLongMessage"
        android:minHeight="48dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button_main"
        app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>

# 5. Intent
# Java
# Alarm
public void createAlarm(String message, int hour, int minutes) {
    Intent intent = new Intent(AlarmClock.ACTION_SET_ALARM)
            .putExtra(AlarmClock.EXTRA_MESSAGE, message)
            .putExtra(AlarmClock.EXTRA_HOUR, hour)
            .putExtra(AlarmClock.EXTRA_MINUTES, minutes);
    if (intent.resolveActivity(getPackageManager()) != null) {
        startActivity(intent);
    }
}

# Maps
public void showMap(Uri geoLocation) {
    Intent intent = new Intent(Intent.ACTION_VIEW);
    intent.setData(geoLocation);
    if (intent.resolveActivity(getPackageManager()) != null) {
        startActivity(intent);
    }
}

# Manifest
# Alarm
<activity ...>
    <intent-filter>
        <action android:name="android.intent.action.SET_ALARM" />
        <category android:name="android.intent.category.DEFAULT" />
    </intent-filter>
</activity>

# Maps
<activity ...>
    <intent-filter>
        <action android:name="android.intent.action.VIEW" />
        <data android:scheme="geo" />
        <category android:name="android.intent.category.DEFAULT" />
    </intent-filter>
</activity>

# 6.Fragment
Gradle Script => build.gradle.kts (Module:app)
plugins {
    id("com.android.application")
}

android {
    namespace = "com.tablayout"
    compileSdk = 34

    defaultConfig {
        applicationId = "com.tablayout"
        minSdk = 21
        targetSdk = 34
        versionCode = 1
        versionName = "1.0"

        testInstrumentationRunner = "androidx.test.runner.AndroidJUnitRunner"
    }

    buildTypes {
        release {
            isMinifyEnabled = false
            proguardFiles(getDefaultProguardFile("proguard-android-optimize.txt"), "proguard-rules.pro")
        }
    }
    compileOptions {
        sourceCompatibility = JavaVersion.VERSION_1_8
        targetCompatibility = JavaVersion.VERSION_1_8
    }
    buildToolsVersion = "34.0.0"
}

dependencies {
    val fragment_version = "1.6.1"
    implementation("androidx.appcompat:appcompat:1.6.1")
    implementation("com.google.android.material:material:1.10.0")
    implementation("androidx.constraintlayout:constraintlayout:2.1.4")
    testImplementation("junit:junit:4.13.2")
    androidTestImplementation("androidx.test.ext:junit:1.1.5")
    androidTestImplementation("androidx.test.espresso:espresso-core:3.5.1")
    implementation("androidx.fragment:fragment:$fragment_version")
}

Setelah itu Sync now
# Java
# MainActivity.java
package com.tablayout;

import androidx.appcompat.app.AppCompatActivity;
import androidx.viewpager2.widget.ViewPager2;

import android.annotation.SuppressLint;
import android.graphics.drawable.ColorDrawable;
import android.os.Bundle;

import com.google.android.material.tabs.TabLayout;

import java.util.Objects;

public class MainActivity extends AppCompatActivity {

    TabLayout tabLayout;
    ViewPager2 viewPager2;
    ViewAdapter adapter;

    @SuppressLint("NewApi")
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Objects.requireNonNull(getSupportActionBar()).setBackgroundDrawable(new ColorDrawable(getColor(R.color.blue)));

        tabLayout = findViewById(R.id.tab);
        viewPager2 = findViewById(R.id.view);
        adapter = new ViewAdapter(this);
        viewPager2.setAdapter(adapter);

        tabLayout.addOnTabSelectedListener(new TabLayout.OnTabSelectedListener() {
            @Override
            public void onTabSelected(TabLayout.Tab tab) {
                viewPager2.setCurrentItem(tab.getPosition());
            }

            @Override
            public void onTabUnselected(TabLayout.Tab tab) {

            }

            @Override
            public void onTabReselected(TabLayout.Tab tab) {

            }
        });

        viewPager2.registerOnPageChangeCallback(new ViewPager2.OnPageChangeCallback() {
            @Override
            public void onPageSelected(int position) {
                super.onPageSelected(position);
                tabLayout.getTabAt(position).select();
            }
        });
    }
}

Membuat file fragment dengan cara klik kanan pada MainActivity.java lalu pilih dan klik fragment, setelah itu pilih dan klik fragment (Blank), setelah itu beri nama ActionFragment, ComedyFragment, RomanceFragment. Untuk file fragment sudah sekaligus dengan file layout xml nya

# Layout Main
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/white"
    tools:context=".MainActivity">


    <com.google.android.material.tabs.TabLayout
        android:id="@+id/tab"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="@color/blue"
        app:tabSelectedTextColor="@color/white"
        app:tabIndicatorColor="@color/white"
        app:tabTextColor="@color/white"
        tools:layout_editor_absoluteX="1dp"
        tools:layout_editor_absoluteY="3dp"
        tools:ignore="MissingConstraints">

        <com.google.android.material.tabs.TabItem
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Action"
            tools:layout_editor_absoluteX="0dp"
            tools:layout_editor_absoluteY="3dp" />

        <com.google.android.material.tabs.TabItem
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Comedy" />

        <com.google.android.material.tabs.TabItem
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Romance" />
    </com.google.android.material.tabs.TabLayout>

    <androidx.viewpager2.widget.ViewPager2
        android:id="@+id/view"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="50dp"
        android:background="@color/white"
        tools:layout_editor_absoluteX="1dp"
        tools:layout_editor_absoluteY="52dp" />

</androidx.constraintlayout.widget.ConstraintLayout>

# ActionFragment.java
package com.tablayout;

import android.os.Bundle;

import androidx.fragment.app.Fragment;

import android.view.LayoutInflater;
import android.view.Menu;
import android.view.MenuInflater;
import android.view.MenuItem;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Toast;


public class ActionFragment extends Fragment {

    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        setHasOptionsMenu(true);
        return inflater.inflate(R.layout.fragment_action, container, false);
    }

    @Override
    public void onCreateOptionsMenu(Menu menu, MenuInflater inflater) {
        inflater.inflate(R.menu.menu_tab, menu);
    }

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        if (item.getItemId() == R.id.tab_action) {
            Toast.makeText(getActivity(), "Clicked on " + item.getTitle(), Toast.LENGTH_SHORT)
                    .show();
        }
        return true;
    }
}

# Layout Action
# fragment_action.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:padding="25dp">

    <ImageView
        android:id="@+id/imgMovie"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:src="@drawable/avatar"/>

    <TextView
        android:id="@+id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="AVATAR : THE WAY OF WATER"/>

    <TextView
        android:id="@+id/Deskription"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="16dp"
        android:maxLines="5"
        android:text="Set more than a decade after the events of the first film, “Avatar: The Way of Water” begins to tell the story of the Sully family (Jake, Neytiri, and their kids), the trouble that follows them, the lengths they go to keep each other safe, the battles they fight to stay alive, and the tragedies they endure."/>
    <ImageView
        android:id="@+id/imgMovie2"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:layout_marginTop="200dp"
        android:src="@drawable/theflash"/>

    <TextView
        android:id="@+id/tvTitle2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:layout_marginTop="200dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="THE FLASH"/>

    <TextView
        android:id="@+id/Deskription2"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="200dp"
        android:maxLines="5"
        android:text="Worlds collide in “The Flash” as Barry uses his superpowers to travel back in time to change past events. But when his efforts to save his family inadvertently alter the future, Barry is trapped in a reality where General Zod has returned, threatening annihilation, and there are no Super Heroes to turn to. That is, unless Barry can coax a very different Batman out of retirement and rescue the imprisoned Kryptonian… although that's not what he's looking for. Ultimately, to save the world he finds himself in and return to the future he knows, Barry's only hope is to race for his life. But will making the ultimate sacrifice be enough to reset the universe?"/>
    <ImageView
        android:id="@+id/imgMovie3"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:layout_marginTop="400dp"
        android:src="@drawable/drstrange"/>

    <TextView
        android:id="@+id/tvTitle3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:layout_marginTop="400dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="DOCTOR STRANGE"/>

    <TextView
        android:id="@+id/Deskription3"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="420dp"
        android:maxLines="5"
        android:text="Dr. Stephen Strange suffered a fatal accident that damaged the motor skills of both hands. For his recovery, he visited a mysterious magician named Ancient One in Tibet."
        />
</RelativeLayout>

# Java Comedy
# ComedyFragment.java
package com.tablayout;

import android.os.Bundle;

import androidx.fragment.app.Fragment;

import android.view.LayoutInflater;
import android.view.Menu;
import android.view.MenuInflater;
import android.view.MenuItem;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Toast;

public class ComedyFragment extends Fragment {

    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        setHasOptionsMenu(true);
        return inflater.inflate(R.layout.fragment_comedy, container, false);
    }

    @Override
    public void onCreateOptionsMenu(Menu menu, MenuInflater inflater) {
        inflater.inflate(R.menu.menu_tab, menu);
    }

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        if (item.getItemId() == R.id.tab_comedy) {
            Toast.makeText(getActivity(), "Clicked on " + item.getTitle(), Toast.LENGTH_SHORT)
                    .show();
        }
        return true;
    }
}

# Layout Comedy
# fragment_comedy.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:padding="25dp">

    <ImageView
        android:id="@+id/imgMovie"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:src="@drawable/mystupidbos"/>

    <TextView
        android:id="@+id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="MY STUPID BOSS"/>

    <TextView
        android:id="@+id/Deskription"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="16dp"
        android:maxLines="5"
        android:text="Due to the crisis of shortage of factory employees, Bossman finally intends to look for new factory employees in Vietnam. Bossman, Diana, Mr. Kho, and Adrian departed for Vietnam. In Vietnam, instead of getting employees, they actually got one problem after another because of Bossman's actions."
        />
    <ImageView
        android:id="@+id/imgMovie2"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:layout_marginTop="200dp"
        android:src="@drawable/okb"/>

    <TextView
        android:id="@+id/tvTitle2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:layout_marginTop="200dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="ORANG KAYA BARU"/>

    <TextView
        android:id="@+id/Deskription2"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="200dp"
        android:maxLines="5"
        android:text="What happens if a family that has been living just barely, suddenly gets abundant wealth? Surely they will be surprised, confused, happy and start buying things that previously only existed in their dreams..."
        />
    <ImageView
        android:id="@+id/imgMovie3"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:layout_marginTop="400dp"
        android:src="@drawable/susahsinyal"/>

    <TextView
        android:id="@+id/tvTitle3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:layout_marginTop="400dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="SUSAH SINYAL"/>

    <TextView
        android:id="@+id/Deskription3"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="420dp"
        android:maxLines="5"
        android:text="Ellen (Adinia Wirasti), a successful lawyer, is a single mom who rarely makes time for her only child Kiara (Aurora Ribero), who eventually grows up as a rebellious teenager who mostly vents her emotions on social media. They live with Agatha (Niniek L. Karim), Ellen's mother who really loves Kiara. When Agatha died of a heart attack, Kiara, who had been very close to her grandmother since childhood, was immediately shaken. The psychologist advised Ellen to take Kiara on holiday, to spend quality time to treat the times when Ellen was too busy working. They went to Sumba, spending fun moments together. Kiara went home with a happy heart. In Jakarta, Ellen was immediately greeted by a big problem at the office. The big project he is working on with Iwan (Ernest Prakasa) is in danger of falling apart. Finally, because she was busy, Ellen didn't keep her promise to watch Kiara perform in the inter-high school talent show competition that Kiara had been preparing for a long time. Kiara was angry and went to Sumba alone, the last place where she could feel a glimmer of happiness. Will Kiara be able to trust her mother again? Will Ellen be able to knit this little family back together? Watch SUSAH SIGNAL, showing in cinemas starting December 21." />
</RelativeLayout>

# Java Romance
# RomanceFragment.java
package com.tablayout;

import android.os.Bundle;

import androidx.fragment.app.Fragment;

import android.view.LayoutInflater;
import android.view.Menu;
import android.view.MenuInflater;
import android.view.MenuItem;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Toast;


public class RomanceFragment extends Fragment {

    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        setHasOptionsMenu(true);
        return inflater.inflate(R.layout.fragment_romance, container, false);
    }
    @Override
    public void onCreateOptionsMenu(Menu menu, MenuInflater inflater) {
        inflater.inflate(R.menu.menu_tab, menu);
    }

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        if (item.getItemId() == R.id.tab_romance) {
            Toast.makeText(getActivity(), "Clicked on " + item.getTitle(), Toast.LENGTH_SHORT)
                    .show();
        }
        return true;
    }
}

# Layout Romance
# fragment_romance.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:padding="25dp">

    <ImageView
        android:id="@+id/imgMovie"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:src="@drawable/ayat2cinta2"/>

    <TextView
        android:id="@+id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginLeft="16dp"
        android:layout_toRightOf="@id/imgMovie"
        android:text="AYAT AYAT CINTA 2"
        android:textColor="@color/black"
        android:textSize="16sp" />

    <TextView
        android:id="@+id/Deskription"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="16dp"
        android:layout_marginTop="16dp"
        android:maxLines="5"
        android:text="The days of FAHRI's life were filled with sorrow and efforts to find the wife he loved so much, AISHA. FAHRI (Fedi Nuril) chooses to live in Edinburgh, Scotland. A city that AISHA really likes. FAHRI works as a respected lecturer and researcher at a well-known university in the city. In living his daily life, FAHRI is only accompanied by HULUSI (Pandji Pragiwaksono), his Turkish household assistant. His politeness and friendly attitude made FAHRI liked by many people, such as Grandma Catarina (Dewi Irawan), a Jewish woman who lived not far from his house. However, there are also those who oppose and even hate him, such as KEIRA (Chelsea Islan), a Scottish-born girl who is obsessed with becoming a famous violinist. One day, FAHRI met HULYA (Tajtana Saphira), a Turkish-German girl who was taking a master's degree in Edinburgh who was still related to AISHA. HULYA's arrival actually triggers FAHRI's sad memories. Can FAHRI achieve its determination to improve the image of Islam and Muslims in this first world country?" />

    <ImageView
        android:id="@+id/imgMovie2"
        android:layout_width="150dp"
        android:layout_height="170dp"
        android:layout_marginTop="200dp"
        android:src="@drawable/ily_from_38_000_ft"/>

    <TextView
        android:id="@+id/tvTitle2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:layout_marginTop="200dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="ILY FROM 38.000 FT"/>

    <TextView
        android:id="@+id/Deskription2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@id/tvTitle"
        android:layout_marginStart="16dp"
        android:layout_marginLeft="12dp"
        android:layout_marginTop="211dp"
        android:layout_toRightOf="@id/imgMovie"
        android:maxLines="5"
        android:text="While on holiday in Bali, Aletta met Arga. The two of them fell in love because they had a lot of chemistry. However, when Aletta decided to return to Jakarta, Arga did not follow her and slowly disappeared from her life." />

    <ImageView
        android:id="@+id/imgMovie3"
        android:layout_width="150dp"
        android:layout_height="175dp"
        android:layout_marginTop="400dp"
        android:src="@drawable/ketikaberhentidisini"/>

    <TextView
        android:id="@+id/tvTitle3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="16dp"
        android:layout_marginTop="400dp"
        android:textSize="16sp"
        android:textColor="@color/black"
        android:text="KETIKA BERHENTI DISINI"/>

    <TextView
        android:id="@+id/Deskription3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@id/tvTitle"
        android:layout_marginStart="16dp"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="409dp"
        android:layout_toRightOf="@id/imgMovie"
        android:maxLines="5"
        android:text="Dita, a graphic designer with high ideals, who is afraid of failure meets Ed, an architect. The meeting, which started with a misunderstanding, ended in a warm conversation. Two people who are similar but not the same come together. Four years since their first meeting, Dita felt that their relationship was going nowhere, without realizing it, Dita always demanded that Ed be what she wanted, but in the end Ed had an accident and died. Dita was devastated and filled with guilt. Two years later, Dita tries to forget everything about Ed and tries to live her new life with Ifan, her best friend since childhood who is now her lover. Not long ago, Dita actually got 'LOOK' glasses with Augmented Reality (AR) technology which can present Ed's figure, exactly the same as real. Will Dita accept Ed's presence again or stay with Ifan?" />
</RelativeLayout>

Buat java class untuk viewadapter.java yang berisi
package com.tablayout;

import androidx.annotation.NonNull;
import androidx.fragment.app.Fragment;
import androidx.fragment.app.FragmentActivity;
import androidx.viewpager2.adapter.FragmentStateAdapter;

public class ViewAdapter extends FragmentStateAdapter {
    public ViewAdapter(@NonNull FragmentActivity fragmentActivity) {
        super(fragmentActivity);
    }

    @NonNull
    @Override
    public Fragment createFragment(int position) {
        switch (position){
            case 0:
                return new ActionFragment();
            case 1:
                return new ComedyFragment();
            case 2:
                return new RomanceFragment();
            default:
                return new ActionFragment();
        }
    }

    @Override
    public int getItemCount() {
        return 3;
    }
}

# Values
# Color.xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="black">#FF000000</color>
    <color name="white">#FFFFFFFF</color>
    <color name="blue">#3700B3</color>
    <color name="pink">#FFC0CB</color>
    <color name="colorPrimary">#3F5185</color>
    <color name="colorPrimaryDark">#303F9F</color>
    <color name="colorAccent">#FF4081</color>
    <color name="birumuda">#ABCBFA</color>
    <color name="salem">#F8C6E6</color>
    <color name ="purple">#E3A2ED</color>
    <color name="hijau">#92A676</color>
    <color name="biru">#8FC2EA</color>
    <color name="hijaumuda">#C2E69C</color>
    <color name="kuning">#FFEB3B</color>
    <color name="orange">#FF9800</color>
    <color name="cream">#E6C18A</color>
    <color name="hijautua">#3F4A2F</color>
</resources>

# Themes
dan untuk themes.xml dan themes.xml(night) berisi code yang sama
<resources xmlns:tools="http://schemas.android.com/tools">
    <!-- Base application theme. -->
    <style name="Base.Theme.TabLayout" parent="Theme.MaterialComponents.DayNight.DarkActionBar">
        <!-- Primary brand color. -->
        <item name="colorPrimary">@color/colorPrimary</item>
        <item name="colorPrimaryVariant">@color/biru</item>
        <item name="colorOnPrimary">@color/white</item>
        <!-- Secondary brand color. -->
        <item name="colorSecondary">@color/blue</item>
        <item name="colorSecondaryVariant">@color/blue</item>
        <item name="colorOnSecondary">@color/blue</item>
        <!-- Status bar color. -->
        <item name="android:statusBarColor">@color/blue</item>
        <item name="android:navigationBarColor">@color/blue</item>
        <!-- Customize your light theme here. -->
    </style>

    <style name="Theme.TabLayout" parent="Base.Theme.TabLayout" />
</resources>

Pada directory drawable kita bisa tambahkan gambar untuk pict dari film yang ingin kita tampilkan, dan jangan lupa untuk menambahkan icon baseline_more_vert_24.xml dengan cara klik kanan pada drawable lalu klik New, setelah itu kita pilih dan klik Vector Asset. Setelah itu kita klik clip art lalu kita pilih icon nya, jika sudah ketemu kita klik OK lalu kita klik next
Selanjutnya kita klik kanan pada app lalu pilih dan klik Android Resource Directory setelah itu kita beri nama "menu" lalu klik OK. Setelah itu kita buat Menu Resource File dengan nama menu_tab.xml lalu isi dengan code :
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:tools="http://schemas.android.com/tools"
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto">
    <item
        android:id="@+id/tab_action"
        android:title="Action"/>

    <item
        android:id="@+id/tab_comedy"
        android:title="Comedy"/>

    <item
        android:id="@+id/tab_romance"
        android:title="Romance"/>
</menu>

# 7. ExoPlayer
# ExoplayerActivity.java
package com.alipapps;

import android.net.Uri;
import android.os.Bundle;
import android.widget.MediaController;
import android.widget.VideoView;
import androidx.annotation.Nullable;
import androidx.appcompat.app.AppCompatActivity;

public class VideoPlayerActivity extends AppCompatActivity {

    @Override
    protected void onCreate(@Nullable Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_video_player);

        // Get the video URI from the intent
        String videoPath = getIntent().getStringExtra("VIDEO_PATH");
        Uri uri = Uri.parse(videoPath);

        // Set up VideoView
        VideoView videoView = findViewById(R.id.videoView);
        videoView.setVideoURI(uri);

        // Set up MediaController
        MediaController mediaController = new MediaController(this);
        mediaController.setAnchorView(videoView);
        videoView.setMediaController(mediaController);

        // Start playing the video
        videoView.start();
    }
}

# Layout activity_exoplayer.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:gravity="center"
    android:background="@color/black">

    <VideoView
        android:id="@+id/videoView"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_centerInParent="true"/>
</RelativeLayout>

# ActionActivity.java
package com.alipapps;

import android.content.Intent;
import android.os.Bundle;
import android.util.Log;
import android.view.LayoutInflater;
import android.view.Menu;
import android.view.MenuInflater;
import android.view.MenuItem;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Button;
import android.widget.Toast;

import androidx.fragment.app.Fragment;

public class ActionFragment extends Fragment {

   private static final String TAG = "ActionFragment";

   @Override
   public View onCreateView(LayoutInflater inflater, ViewGroup container,
                            Bundle savedInstanceState) {
       // Inflate the layout for this fragment
       setHasOptionsMenu(true);
       View view = inflater.inflate(R.layout.fragment_action, container, false);

       // Find the button by its ID
       Button avatarButton = view.findViewById(R.id.avatar);
       Button theflashButton = view.findViewById(R.id.theflash);
       Button drstrangeButton = view.findViewById(R.id.drstrange);

       // Set click listener for each button
       avatarButton.setOnClickListener(new View.OnClickListener() {
           @Override
           public void onClick(View v) {
               Log.d(TAG, "Avenger button clicked");
               playVideo(R.raw.avatar);
           }
       });

       theflashButton.setOnClickListener(new View.OnClickListener() {
           @Override
           public void onClick(View v) {
               Log.d(TAG, "MyName button clicked");
               playVideo(R.raw.theflash);
           }
       });

       drstrangeButton.setOnClickListener(new View.OnClickListener() {
           @Override
           public void onClick(View v) {
               Log.d(TAG, "Spiderman button clicked");
               playVideo(R.raw.drstrange);
           }
       });

       return view;
   }

   @Override
   public void onCreateOptionsMenu(Menu menu, MenuInflater inflater) {
       inflater.inflate(R.menu.menu_tab, menu);
   }

   @Override
   public boolean onOptionsItemSelected(MenuItem item) {
       if (item.getItemId() == R.id.tab_action) {
           Toast.makeText(getActivity(), "Clicked on " + item.getTitle(), Toast.LENGTH_SHORT)
                   .show();
       }
       return true;
   }

   private void playVideo(int videoResource) {
       String videoPath = "android.resource://" + getActivity().getPackageName() + "/" + videoResource;
       Intent intent = new Intent(getActivity(), VideoPlayerActivity.class);
       intent.putExtra("VIDEO_PATH", videoPath);
       startActivity(intent);
   }
}
# Layout activity_action.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    xmlns:tools="http://schemas.android.com/tools"
    android:padding="25dp"
    tools:context=".ActionFragment">


    <ImageView
        android:id="@+id/imgMovie"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="5dp"
        android:src="@drawable/avatar" />

    <TextView
        android:id="@+id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_alignParentEnd="true"
        android:layout_marginStart="10dp"
        android:layout_marginTop="5dp"
        android:layout_toRightOf="@id/imgMovie"
        android:text="AVATAR : THE WAY OF WATER"
        android:textColor="@color/black"
        android:textSize="14sp" />

    <TextView
        android:id="@+id/Deskription"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tvTitle"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:maxLines="5"
        android:text="Set more than a decade after the events of the first film, “Avatar: The Way of Water” begins to tell the story of the Sully family (Jake, Neytiri, and their kids), the trouble that follows them, the lengths they go to keep each other safe, the battles they fight to stay alive, and the tragedies they endure."
        android:textColor="@color/black"
        android:textSize="14sp" />


    <Button
        android:id="@+id/avatar"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/Deskription"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playAvatarTrailer"/>


    <ImageView
        android:id="@+id/imgMovie2"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="190dp"
        android:src="@drawable/theflash" />

    <TextView
        android:id="@+id/tvTitle2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie2"
        android:layout_marginStart="10dp"
        android:layout_marginTop="190dp"
        android:textSize="15sp"
        android:textColor="@color/black"
        android:text="THE FLASH"/>

    <TextView
        android:id="@+id/Deskription2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tvTitle2"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie2"
        android:maxLines="5"
        android:text="Worlds collide in “The Flash” as Barry uses his superpowers to travel back in time to change past events. But when his efforts to save his family inadvertently alter the future, Barry is trapped in a reality where General Zod has returned, threatening annihilation, and there are no Super Heroes to turn to. That is, unless Barry can coax a very different Batman out of retirement and rescue the imprisoned Kryptonian… although that's not what he's looking for. Ultimately, to save the world he finds himself in and return to the future he knows, Barry's only hope is to race for his life. But will making the ultimate sacrifice be enough to reset the universe?"
        android:textColor="@color/black"
        android:textSize="14sp" />

    <Button
        android:id="@+id/theflash"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie2"
        android:layout_below="@id/Deskription2"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playTheflashTrailer"/>

    <ImageView
        android:id="@+id/imgMovie3"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="380dp"
        android:src="@drawable/drstrange" />

    <TextView
        android:id="@+id/tvTitle3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie3"
        android:layout_marginStart="10dp"
        android:layout_marginTop="380dp"
        android:textSize="15sp"
        android:textColor="@color/black"
        android:text="DOCTOR STRANGE"/>

    <TextView
        android:id="@+id/Deskription3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tvTitle3"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie3"
        android:maxLines="5"
        android:text="Dr. Stephen Strange suffered a fatal accident that damaged the motor skills of both hands. For his recovery, he visited a mysterious magician named Ancient One in Tibet."
        android:textColor="@color/black"
        android:textSize="15sp" />

    <Button
        android:id="@+id/drstrange"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie3"
        android:layout_below="@id/Deskription3"
        android:text="Watch Trailer Now"
        android:textSize="12sp"
        android:onClick="playDrstrangeTrailer" />

</RelativeLayout>
# ComedyActivity.java
package com.alipapps;

import android.content.Intent;
import android.os.Bundle;
import android.util.Log;
import android.view.LayoutInflater;
import android.view.Menu;
import android.view.MenuInflater;
import android.view.MenuItem;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Button;
import android.widget.Toast;

import androidx.fragment.app.Fragment;

public class ComedyFragment extends Fragment {

   private static final String TAG = "ComedyFragment";

   @Override
   public View onCreateView(LayoutInflater inflater, ViewGroup container,
                            Bundle savedInstanceState) {
       // Inflate the layout for this fragment
       setHasOptionsMenu(true);
       View view = inflater.inflate(R.layout.fragment_comedy, container, false);

       // Find the button by its ID
       Button mystupidbossButton = view.findViewById(R.id.mystupidboss);
       Button orangkayabaruButton = view.findViewById(R.id.okb);
       Button susahsinyalButton = view.findViewById(R.id.susahsinyal);

       // Set click listener for each button
       mystupidbossButton.setOnClickListener(new View.OnClickListener() {
           @Override
           public void onClick(View v) {
               Log.d(TAG, "Mt stupid boss button clicked");
               playVideo(R.raw.mystupidboss);
           }
       });

       orangkayabaruButton.setOnClickListener(new View.OnClickListener() {
           @Override
           public void onClick(View v) {
               Log.d(TAG, "Orang kaya baru button clicked");
               playVideo(R.raw.orangkayabaru);
           }
       });

       susahsinyalButton.setOnClickListener(new View.OnClickListener() {
           @Override
           public void onClick(View v) {
               Log.d(TAG, "Susah sinyal button clicked");
               playVideo(R.raw.susahsinyal);
           }
       });

       return view;
   }

   @Override
   public void onCreateOptionsMenu(Menu menu, MenuInflater inflater) {
       inflater.inflate(R.menu.menu_tab, menu);
   }

   @Override
   public boolean onOptionsItemSelected(MenuItem item) {
       if (item.getItemId() == R.id.tab_comedy) {
           Toast.makeText(getActivity(), "Clicked on " + item.getTitle(), Toast.LENGTH_SHORT)
                   .show();
       }
       return true;
   }

   private void playVideo(int videoResource) {
       String videoPath = "android.resource://" + getActivity().getPackageName() + "/" + videoResource;
       Intent intent = new Intent(getActivity(), VideoPlayerActivity.class);
       intent.putExtra("VIDEO_PATH", videoPath);
       startActivity(intent);
   }
}

# Layout activity_comedy.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:padding="25dp">

    <ImageView
        android:id="@+id/imgMovie"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="5dp"
        android:src="@drawable/mystupidbos" />

    <TextView
        android:id="@+id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_marginStart="10dp"
        android:layout_marginTop="5dp"
        android:layout_toRightOf="@id/imgMovie"
        android:text="MY STUPID BOSS"
        android:textColor="@color/black"
        android:textSize="15sp" />

    <TextView
        android:id="@+id/Deskription"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:textSize="14sp"
        android:maxLines="5"
        android:text="Due to the crisis of shortage of factory employees, Bossman finally intends to look for new factory employees in Vietnam. Bossman, Diana, Mr. Kho, and Adrian departed for Vietnam. In Vietnam, instead of getting employees, they actually got one problem after another because of Bossman's actions."
        />

    <Button
        android:id="@+id/mystupidboss"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/Deskription"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playMystupidbossTrailer"/>

    <ImageView
        android:id="@+id/imgMovie2"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="195dp"
        android:src="@drawable/okb" />

    <TextView
        android:id="@+id/tvTitle2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="10dp"
        android:layout_marginTop="195dp"
        android:textSize="15sp"
        android:textColor="@color/black"
        android:text="ORANG KAYA BARU"/>

    <TextView
        android:id="@+id/Deskription2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tvTitle2"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:maxLines="5"
        android:text="What happens if a family that has been living just barely, suddenly gets abundant wealth? Surely they will be surprised, confused, happy and start buying things that previously only existed in their dreams..."
        android:textSize="14sp" />

    <Button
        android:id="@+id/okb"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/Deskription2"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playOrangkayabaruTrailer"/>

    <ImageView
        android:id="@+id/imgMovie3"
        android:layout_width="110dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_marginTop="385dp"
        android:src="@drawable/koalakumal" />

    <TextView
        android:id="@+id/tvTitle3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="10dp"
        android:layout_marginTop="385dp"
        android:textSize="15sp"
        android:textColor="@color/black"
        android:text="KOALA KUMAL"/>

    <TextView
        android:id="@+id/Deskription3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tvTitle3"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:maxLines="5"
        android:text="KOALA KUMAL is still telling the story of Dika, a guy who just canceled his marriage because his girlfriend, Andrea, cheated on him with a guy named James. His broken heart made it difficult for Dika to write the last chapter of his book. One day, Dika met a girl named Trishna, a unique girl who made Dika's perspective on the world different."
        android:textSize="14sp" />

    <Button
        android:id="@+id/susahsinyal"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/Deskription3"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playSusahsinyalTrailer"/>
</RelativeLayout>

# RomanceActivity.java
package com.alipapps;

import android.content.Intent;
import android.os.Bundle;
import android.util.Log;
import android.view.LayoutInflater;
import android.view.Menu;
import android.view.MenuInflater;
import android.view.MenuItem;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Button;
import android.widget.Toast;

import androidx.fragment.app.Fragment;

public class RomanceFragment extends Fragment {

    private static final String TAG = "RomanceFragment";

    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        setHasOptionsMenu(true);
        View view = inflater.inflate(R.layout.fragment_romance, container, false);

        // Find the button by its ID
        Button ayatayatcinta2Button = view.findViewById(R.id.ayatayatcinta2);
        Button ilyfrom38000ftButton = view.findViewById(R.id.iloveyoufrom38000ft);
        Button ketikaberhentidisniButton = view.findViewById(R.id.ketikaberhentidisini);

        // Set click listener for each button
        ayatayatcinta2Button.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Log.d(TAG, "Ayat ayat cinta 2 button clicked");
                playVideo(R.raw.ayatayatcinta2);
            }
        });

        ilyfrom38000ftButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Log.d(TAG, "I love from 38.000 ft button clicked");
                playVideo(R.raw.ilyfrom38000ft);
            }
        });

        ketikaberhentidisniButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Log.d(TAG, "Ketika berhenti disini button clicked");
                playVideo(R.raw.ketikaberhentidisini);
            }
        });

        return view;
    }

    @Override
    public void onCreateOptionsMenu(Menu menu, MenuInflater inflater) {
        inflater.inflate(R.menu.menu_tab, menu);
    }

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        if (item.getItemId() == R.id.tab_romance) {
            Toast.makeText(getActivity(), "Clicked on " + item.getTitle(), Toast.LENGTH_SHORT)
                    .show();
        }
        return true;
    }

    private void playVideo(int videoResource) {
        String videoPath = "android.resource://" + getActivity().getPackageName() + "/" + videoResource;
        Intent intent = new Intent(getActivity(), VideoPlayerActivity.class);
        intent.putExtra("VIDEO_PATH", videoPath);
        startActivity(intent);
    }
}

# Layout activity_romace.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:padding="25dp">

    <ImageView
        android:id="@+id/imgMovie"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="5dp"
        android:src="@drawable/ayat2cinta2" />

    <TextView
        android:id="@+id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_marginStart="10dp"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="5dp"
        android:layout_toRightOf="@id/imgMovie"
        android:text="AYAT AYAT CINTA 2"
        android:textColor="@color/black"
        android:textSize="15sp" />

    <TextView
        android:id="@+id/Deskription"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/tvTitle"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:textSize="14sp"
        android:maxLines="5"
        android:text="The days of FAHRI's life were filled with sorrow and efforts to find the wife he loved so much, AISHA. FAHRI (Fedi Nuril) chooses to live in Edinburgh, Scotland. A city that AISHA really likes. FAHRI works as a respected lecturer and researcher at a well-known university in the city. In living his daily life, FAHRI is only accompanied by HULUSI (Pandji Pragiwaksono), his Turkish household assistant. His politeness and friendly attitude made FAHRI liked by many people, such as Grandma Catarina (Dewi Irawan), a Jewish woman who lived not far from his house. However, there are also those who oppose and even hate him, such as KEIRA (Chelsea Islan), a Scottish-born girl who is obsessed with becoming a famous violinist. One day, FAHRI met HULYA (Tajtana Saphira), a Turkish-German girl who was taking a master's degree in Edinburgh who was still related to AISHA. HULYA's arrival actually triggers FAHRI's sad memories. Can FAHRI achieve its determination to improve the image of Islam and Muslims in this first world country?" />

    <Button
        android:id="@+id/ayatayatcinta2"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/Deskription"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playAyatayatcinta2Trailer"/>

    <ImageView
        android:id="@+id/imgMovie2"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="190dp"
        android:src="@drawable/ily_from_38_000_ft" />

    <TextView
        android:id="@+id/tvTitle2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="10dp"
        android:layout_marginTop="190dp"
        android:textSize="15sp"
        android:textColor="@color/black"
        android:text="ILY FROM 38.000 FT"/>

    <TextView
        android:id="@+id/Deskription2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tvTitle2"
        android:layout_marginStart="10dp"
        android:layout_marginLeft="12dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:maxLines="5"
        android:text="While on holiday in Bali, Aletta met Arga. The two of them fell in love because they had a lot of chemistry. However, when Aletta decided to return to Jakarta, Arga did not follow her and slowly disappeared from her life."
        android:textSize="14sp" />

    <Button
        android:id="@+id/iloveyoufrom38000ft"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/Deskription2"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playIlyfrom38000ftTrailer"/>

    <ImageView
        android:id="@+id/imgMovie3"
        android:layout_width="120dp"
        android:layout_height="160dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_marginTop="380dp"
        android:src="@drawable/ketikaberhentidisini" />

    <TextView
        android:id="@+id/tvTitle3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_marginStart="10dp"
        android:layout_marginTop="380dp"
        android:textSize="15sp"
        android:textColor="@color/black"
        android:text="KETIKA BERHENTI DISINI"/>

    <TextView
        android:id="@+id/Deskription3"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/tvTitle3"
        android:layout_marginStart="10dp"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:maxLines="5"
        android:text="Dita, a graphic designer with high ideals, who is afraid of failure meets Ed, an architect. The meeting, which started with a misunderstanding, ended in a warm conversation. Two people who are similar but not the same come together. Four years since their first meeting, Dita felt that their relationship was going nowhere, without realizing it, Dita always demanded that Ed be what she wanted, but in the end Ed had an accident and died. Dita was devastated and filled with guilt. Two years later, Dita tries to forget everything about Ed and tries to live her new life with Ifan, her best friend since childhood who is now her lover. Not long ago, Dita actually got 'LOOK' glasses with Augmented Reality (AR) technology which can present Ed's figure, exactly the same as real. Will Dita accept Ed's presence again or stay with Ifan?"
        android:textSize="14sp" />

    <Button
        android:id="@+id/ketikaberhentidisini"
        android:layout_width="wrap_content"
        android:layout_height="40dp"
        android:layout_marginStart="10dp"
        android:layout_marginTop="10dp"
        android:layout_toRightOf="@id/imgMovie"
        android:layout_below="@id/Deskription3"
        android:text="Watch Trailer Now"
        android:textSize="10sp"
        android:onClick="playKetikaberhentidisiniTrailer"/>

</RelativeLayout>


# SEKIAN
