# qTest Automation SDK
This package includes automation libraries and automation host
developer edition.

### Automation libraries
* agent-base-1.0.0.jar - including plugin domain classes, plugin
  utilities.
* agent-plugin-access.jar - including plugin extension and some domain
  classes.
* agent-plugin-api-1.0.0.jar - incluing plugin API use to develop
  automation plugin.
* qtest-sdk-java-1.1.3.jar - including qTest API SDK and qTest API
  domain classes.
* External libraries:
  * commons-lang-2.6.jar
  * commons-codec-1.10.jar
  * commons-io-2.4.jar
  * jackson-core-2.5.1.jar
  * jackson-annotations-2.5.1.jar
  * commons-logging-1.1.3.jar
  * log4j-1.2.17.jar

### Automation Host Developer Edition
###### Run
```sh
$ cd agent
$ java -jar agent.jar
```
In the first time, Automation Host applies the database and generate
the folder structure:
* config: the automation host configuration folder.
* db: the automation host database.
* lib: the additional libraries.
* plugins: internal (bundled) and external plugin.
* plugins_work: plugin installed directory.

###### Install plugin
* Copy plugin (jar file) to plugins/external of Automation Host
* Restart Automation Host to take effect.

###### Uninstall plugin
* Remove your plugin folder in plugins_work folder of Automation Host
* Remove your plugin file (jar file) in plugins/external
