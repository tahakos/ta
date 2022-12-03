# ta
MP ODEV TK
package com.example.mptkodev

import android.R
import android.os.Bundle
import android.widget.EditText
import androidx.appcompat.app.AppCompatActivity


class MainActivity : AppCompatActivity() {
    var editText_sayi1: EditText? = null
    var editText_sayi2: EditText? = null
    var button: Button? = null
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
        button = findViewById(R.id.button_Kontrol)
        editText_sayi1 = findViewById(R.id.editTextNumber_Sayi1)
        editText_sayi2 = findViewById(R.id.editTextNumber_Sayi2)

        public void kontrol(View view){
            int sayi1 = Integer.parseInt(editText_sayi1.getText().toString());
            val value = int sayi2 = Integer . parseInt (editText_sayi2.getText().toString());
            if(sayi1>sayi2){
                Toast.makeText(MainActivity.this,”1. Sayı Daha Büyüktür.”,Toast.LENGTH_
                LONG).show();
            }
            if(sayi2>sayi1){
                Toast.makeText(MainActivity.this,”2. Sayı Daha Büyüktür.”,Toast.LENGTH_
                LONG).show();
            }
            if(sayi1==sayi2){
                Toast.makeText(MainActivity.this,”İki Sayı Birbirine Eşittir.”,Toast.LENGTH_LONG).show();
            }
        }
    }
}
