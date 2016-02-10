# Structure #
```
<command>
 <command/>
 <host/>
 <port/>	
 <bindPreferences/>
 <earFile/>
 <appName/>
 <target/>
 <username/>
 <password/>
 <eableSecurity/>
 <trustStoreFile/>
 <trustStorePassword/>
 <keyStoreFile/>
 <keyStorePassword/>
 <description/>
 <stopOnError/>
 <pathAppClient/>
 <ibmJre/>
</command>
```

# Details #

**command**
  * command to execute
  * type: enum { INSTALL, START, STOP, UNINSTALL }

**host**
  * target hostname
  * type: String
  * INSTALL: required
  * START: required
  * STOP: required
  * UNINSTALL: required

**port**
  * websphere soap port
  * type Integer
  * INSTALL: required
  * START: required
  * STOP: required
  * UNINSTALL: required

**bindPreferences**
  * binding preferences, es: { defaultbinding.virtual.host=default\_host ]
  * type java.util.Properties
  * INSTALL: optional
  * START: optional
  * STOP: optional
  * UNINSTALL: optional

**earFile**
  * ear path
  * type: String
  * INSTALL: required
  * START: optional
  * STOP: optional
  * UNINSTALL: optional

**appName**
  * installation app name
  * type: String
  * INSTALL: required
  * START: required
  * STOP: required
  * UNINSTALL: required

**target**
  * websphere target
  * type: String
  * INSTALL: required
  * START: required
  * STOP: required
  * UNINSTALL: required

**username**

**password**

**eableSecurity**

**trustStoreFile**

**trustStorePassword**

**keyStoreFile**

**keyStorePassword**

**description**
  * type: String
  * INSTALL: optional
  * START: optional
  * STOP: optional
  * UNINSTALL: optional

**stopOnError**
  * if false ignore error and continue
  * type: boolean
  * default: false
  * INSTALL: optional
  * START: optional
  * STOP: optional
  * UNINSTALL: optional

**pathAppClient**
  * path to IBM Websphere Application Client
  * type: String
  * INSTALL: required
  * START: required
  * STOP: required
  * UNINSTALL: required

**ibmJre**
  * path to IBM Websphere jre
  * type: String
  * default: use jre on pathAppClient
  * INSTALL: optional
  * START: optional
  * STOP: optional
  * UNINSTALL: optional

[Summary](Summary.md)