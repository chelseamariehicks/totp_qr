Instructions for how to run the program:
-no makefile was provided since the program was written in Python and can be run with the following 
command:

    -python totp_qr.py

Implementation process:

I began by researching libraries for qr code generation and one-time password generation. Since Python
has both of these, I selected that as my language for the assignment and installed both libraries on my
system: pip install qrcode and pip install pyotp.

From there, I was able to review documentation to identify how to encode the URI Google Authenticator expects
in the QR code as well as how to generate the QR code using the Python library. 


Assumptions:
-User id for URI can be whatever I want it to be, in this case I choose: pharaohcious@egyptiancats.com
-Secret key can be hard coded, I went with this not secret, randomly generated key: 3A5QCZTNABFSY777
-Commands --generate-qr and --get-otp can be treated as input and entered after the program is running
-Testing using iOS Google Authenticator is sufficient given statement in program specs that: 
"Functionality wise, Android and iOS apps are supposed to provide similar codes"
-It's acceptable for the implementation to have the OTP print up to 10 times before program returns
-QR code can be saved as .jpg in program folder

Future improvements:
-Take validated user input for user id to make this more dynamic
-Generate a new, random secret key each time program is run
-Try different color combos for the QR code
