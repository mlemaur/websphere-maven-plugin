[Summary](Summary.md)

Websphere Maven Plugin provides goals to:

  1. deploy ear on websphere 7
  1. start application
  1. stop application
  1. uninstall


require websphere application client.

[download](http://code.google.com/p/websphere-maven-plugin/source/browse/trunk/plugin/)

Example:
```
<plugin>
 <groupId>Websphere7AM.plugin</groupId>
 <artifactId>websphere7am-maven-plugin</artifactId>
 <version>1.0.0</version>
 
 <configuration>
  <defaultCommand>
   <host>localhost</host>
   <port>8880</port>
  </defaultCommand>
  <commands>
   <command>
    <command>INSTALL</command>
    <appName>My Application</appName>
    <earFile>myapp.ear</earFile>
    <target>WebSphere:cell=myhostNode01Cell,node=myhostNode01,server=server1</target>
    <description>Install my app</description>
   </command>
  </commands>
 </configuration>

 <executions>
  <execution>
   <phase>compile</phase>
   <goals>
    <goal>was</goal>
   </goals>
  </execution>
 </executions>

</plugin>
```