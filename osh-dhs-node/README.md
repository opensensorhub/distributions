### DHS Demo Field Node

OSH distribution used on the field node computer for the DHS emergency response testbed.


#### Startup

To start using OSH with the default configuration, just run the command:

    ./launch.sh

If you want to run it on a server through SSH and keep the process running when you log-out, use

    nohup ./launch &


#### Web Admin User Interface

After launching OSH, you can connect to the admin UI at:
<http://localhost:8181/sensorhub/admin>

or view the SOS server capabilities at:
<http://localhost:8181/sensorhub/sos?service=SOS&version=2.0&request=GetCapabilities>
