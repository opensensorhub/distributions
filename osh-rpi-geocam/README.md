### Geospatially Aware Video Camera with Raspberry Pi

OSH distribution with preloaded drivers for creating a geospatially aware camera using a Raspberry Pi and and off-the-shelf components. This includes sensor drivers for NMEA GPS, BNO055 absolute orientation sensor and Video4Linux camera.



#### Build

Run `mvn clean install` in this folder. This will build a ZIP file that's ready to extract on your Raspberry Pi.



#### Startup

To start using OSH with the default configuration, just run the command:

>> ./launch.sh


If you want to run it on a server through SSH and keep the process running when you log-out, use

>> nohup ./launch &



#### Admin

After launching OSH, you can connect to the admin console:
http://localhost:8181/sensorhub/admin

or view the SOS server capabilities at:
http://localhost:8181/sensorhub/sos?service=SOS&version=2.0&request=GetCapabilities



#### Test Web Clients

You can also try the included javascript clients connecting to the SOS server.
These are very simple web pages intended to provide examples of how to efficiently render the data
streamed by the SOS server.

http://localhost:8181/osm_client_websockets.html
