restart-pentaho
===============

* PDI job that restart the service of Pentaho BI-Server

**Usage**

Execute the job job_restart_pentaho.kjb 

You should pass two parameters:

* SERVER_PATH -> Path of your bi-server.

* TIMEOUT -> Time in minutes that the start-pentaho.sh should execute after stop-pentaho.sh is executed

Example.

sh kitchen.sh -file="job_restart_pentaho.kjb"  --level=Debug -param="SERVER_PATH=/opt/pentaho/biserver/biserver-ce/" -param="TIMEOUT=1"
