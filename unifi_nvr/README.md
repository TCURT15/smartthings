# Ubiquiti UniFi Video NVR for Samsung SmartThings
This is a SmartApp that will discover cameras from your NVR and create child devices for each camera.

The API for the NVR is not published by Ubiquiti so this integration is subject to break, however unlikely.  

To use the app, you must have an active API key from a user with proper permissions.  In the NVR software click on "Users", select a user (probably your super administrator) then select "API Access".  Make sure that "Allow API Usage" is enabled then copy the API key into the app settings.

Your SmartThings hub running this SmartApp must be on the same subnet as the NVR software.  This is a restriction of the hub that it will not perform HTTP GET commands outside the subnet.  The hub also does not currently support HTTPS interactions so ensure that the network is trusted.

I have tested this against NVR v3.5.2 and a UVC G3 Dome.