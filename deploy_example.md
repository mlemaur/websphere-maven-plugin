# Deploy example #

```
<command>
 <name>Install</name>
 <description>My Ear</description>
 <command>INSTALL</command>
 <host>localhost</host>
 <port>8880</port>
 <appName>My app name</appName>
 <earFile>/rad/target/myEAR-1.3.3.ear</earFile
 <target>WebSphere:cell=myserverNode01Cell,node=myserverNode01,server=server1</target>
 <pathAppClient>/IBM/WebSphere/AppClient</pathAppClient>	
 <bindProperties>
  <property>
   <name>defaultbinding.virtual.host</name>
   <value>default_host</value>
  </property>
 </bindProperties>
</command>
```

[Summary](Summary.md)