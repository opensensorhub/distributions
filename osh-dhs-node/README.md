### DHS Demo Field Node

OSH distribution used on the field node computer for the DHS emergency response testbed.


#### Build

To build this distribution, just clone the needed repositories and run a Gradle build:

```
$ git clone --recursive https://github.com/opensensorhub/osh-core
$ git clone https://github.com/opensensorhub/osh-comm
$ git clone https://github.com/opensensorhub/osh-sensors
$ git clone https://github.com/opensensorhub/osh-services
$ git clone https://github.com/opensensorhub/osh-distros
$ cd osh-distros/osh-dhs-node/
$ ../gradlew build
```

The resulting Zip file is in the `build/distributions` folder. Just unzip it and run with Java version >= 7.


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
