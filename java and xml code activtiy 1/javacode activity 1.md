{

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
       final Intent i = new Intent(MainActivity.this, day4cw2part2.class);
        EditText name = findViewById(R.id.yourname);
        EditText age = findViewById(R.id.yourage);
        Button next = findViewById(R.id.button);
        next.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                String data = name.getText().toString();
                String number = age.getText().toString();
                i.putExtra("bagdata",data);
                i.putExtra("data2" , number);
                startActivity(i);
            }
        });
    }
}