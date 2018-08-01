## DOCKER CI STACK


This is a **docker continuous integration stack** , it wraps Jenkins, SonarQube and Nexus all in different images that will be instanciated to containers after.
Make sure yourve Docker installed , then cd into the directory and run "Docker-compose up".
once the dependencies are downloaded, you can visit the servers with the designtaed ports by adding a "1" to the left of the default ports,  as follows:

1. Jenkins : 18080
2. Nexus : 19001
3. SonarQube : 19000

the server address is the default docker machine IP created by the VM.

Then make sure the jobs directory has Jenkins permissions and NOT root.

PS : There is a shared folder called Jobs inside jenkins/jenkins-data; it was made for consistency so jobs arent lost when containers are destroyed.
