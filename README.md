# BandSDKTest
Android Test Application for the Microsoft Band SDK Preview. Sorry for any crap code or anything that's wrong, this is a hack-it-up playground.

## Notes That Are Important
First off, you need to follow the readme.txt instructions for adding the library to android studio. If you do an import module, it will result in all sorts of un-resolved externals. Instead, follow the instructions and it works fine:

    First, include the Microsoft Band SDK jar file in your Android project.  To do
    that in Android Studio:
    - Go to your Android project's application directory and locate the libs 
      folders (you can create it if it does not already exist), and copy the jar
      file to this location.
    - Open the Project Structure window from the File menu
    - Select the application module from the Modules list on the left
    - Select the Dependencies tab on the right
    - Click the + button on the right and select File dependency
    - Expand the libs folder, select the jar file, and click OK

The API for **com.microsoft.band.BandConnectionResult** doesn't appear to exist but is listed. I think instead you need to use **com.microsoft.band.BandConnectionState** and pull a result from that.
