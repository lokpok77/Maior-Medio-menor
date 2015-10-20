package com.eedgar.exe10;




import android.os.Bundle;
import android.app.Activity;
import android.view.Menu;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;

public class MainActivity extends Activity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }


    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        // Inflate the menu; this adds items to the action bar if it is present.
        getMenuInflater().inflate(R.menu.main, menu);
        return true;
    }
    
    public void dez (View v){
    	
    
    	
    	
    			EditText primeiro=(EditText)findViewById(R.id.entPrimeiro);
    				String stringPrimeiro = primeiro.getText().toString();
    				int a =  Integer.parseInt(stringPrimeiro);

    			EditText segundo=(EditText)findViewById(R.id.entSegundo);
    				String stringSegundo = segundo.getText().toString();
    				int b = Integer.parseInt(stringSegundo);
	
    			EditText terceiro=(EditText)findViewById(R.id.entTerceiro);
    				String stringTerceiro = terceiro.getText().toString();
    				int c = Integer.parseInt(stringTerceiro);
    				
    				
    				int maior = 1;
    				int medio = 2;
    				int menor = 3;
    				
    				
    				
    				if (a > b ) {
    					maior = a;	
    				}
    				
    				else if (( a < b) && (a > b) ){
    					medio = a;
    				}
    				
    				else { 
    					menor = a;
    				}
    				//......................................
    				
    				if (b > a) {
    					maior = b;
    				}
    				
    				else if (( b < a) && (b > a)) {
    					medio = b;
    				}
    				
    				else {
    					menor = b;
    				}
    				//...........................................
    				
    				if (c > a){
    					maior = c;
    				}
    				
    				else if ((c < a) && (c > a)) {
    					medio = c;
    				}
    				
    				else { 
    					menor = c;
    				//..............................	
    				}
    				
    				if (c > b){
    					maior = c;
    				}
    				
    				else if ((c < b) && (c > b)){
    					medio = c;
    				}
    				
    				else { 
    					menor = c;
    				}
    				
    				
    				TextView TxResultado = (TextView)findViewById(R.id.entResultado);
    				TxResultado.setText(" Maior " + maior + " Medio " + medio  + " Menor " + menor);
    }
 }				
 
