package com.example.day4cw1;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.TextView;

public class day4cw2part2 extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_day4cw2part2);
        TextView myname = findViewById(R.id.myname);
        TextView myage = findViewById(R.id.myage);
        Bundle bundle = getIntent().getExtras();
        Bundle bundle2 = getIntent().getExtras();
       String mybagdata = bundle.getString("bagdata");
        String mydata2 = bundle2.getString("data2");
        myname.setText(mybagdata);
        myage.setText(mydata2);


    }
}
