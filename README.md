Generate QR code from various files and verify the authenticity of the file using digital signature.

AuthenticQR is the source for the android app

The bin folder inside Authentic QR should not be modified

The digital signatute scheme has been implemented using:

-> Encryption Algorithm: RSA

-> Hash Algorithm: SHA-256, Provider: Bouncycastle(PC), Spongycastle(app)

-> Keysize: 3072-bit

System requirements for PC:

-> Linux

-> JDK 1.7 and above

-> GTK+

-> gtkdialog

-> zenity

Start the GUI by executing start.sh via the terminal(Ex: foo@bar:~$ sh start.sh )
Alternatively change the permission of 'start.sh' & make it executable($ chmod +x start.sh) for once. Then like any other app, just double click on start.sh to run the GUI.

# ANDROID APP

SecuredQR is the source for the android app. The app can be used to generate QRCode image and digital signature, public key similar to the PC version.

The scan feature of the app is restricted to scanning QRCodes of zip files that contain a file, its detached digital signature('sig') and the public key('suepk') only.
Any other QRCode scanning will result in an error which will be displayed on the screen!

Decoding any QRCode is also possible via the app!

Android smartphone requirements:

-> Android API 17 or above

-> BarcodeScanner app by zxing

-> A good built-in camera

-> Good CPU and RAM
