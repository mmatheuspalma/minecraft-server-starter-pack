## Minecraft Server

### Requirements
- Java
- Java JDK
- Ngrok

### Running

#### Starting server
Open terminal on folder and start the minecraft server
````shell
    java -server -Xmx2048M -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:+CMSIncrementalPacing -XX:ParallelGCThreads=2 -XX:+AggressiveOpts -jar server.jar
````

#### Let's create a tunnel for your local network 
After start server, open the ngrok application, and type
````shell
    ngrok tcp the_server_port --region us 
````

After this, copy the url and share with us