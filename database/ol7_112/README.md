# Oracle 11.2 on Oracle Linux 7

A simple Vagrant build for Oracle Database 11.2 on Oracle Linux 7.

## Required Software

* [Vagrant](https://www.vagrantup.com/downloads.html)
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Oracle Database](https://edelivery.oracle.com)
* [Oracle REST Data Services (ORDS)](https://www.oracle.com/technetwork/developer-tools/rest-data-services/downloads/)
* [Oracle SQLcl](https://www.oracle.com/tools/downloads/sqlcl-downloads.html)
* [Oracle Application Express (APEX)](https://www.oracle.com/tools/downloads/apex-downloads.html)
* [OpenJDK 11](https://adoptium.net/releases.html?variant=openjdk11&jvmVariant=hotspot)
* [Tomcat 9](https://tomcat.apache.org/download-90.cgi)

Place the Oracle database software in the "software" directory before calling the `vagrant up` command.

Directory contents when software is included.

```
$ tree
.
+--- config
|   +--- install.env
|   +--- vagrant.yml
+--- README.md
+--- scripts
|   +--- dbora.service
|   +--- install_os_packages.sh
|   +--- oracle_create_database.sh
|   +--- oracle_service_setup.sh
|   +--- oracle_software_installation.sh
|   +--- oracle_user_environment_setup.sh
|   +--- ords_software_installation.sh
|   +--- root_setup.sh
|   +--- server.xml
|   +--- setup.sh
+--- software
|   +--- apache-tomcat-9.0.62.tar.gz
|   +--- apex_21.1_en.zip
|   +--- p13390677_112040_Linux-x86-64_1of7.zip
|   +--- p13390677_112040_Linux-x86-64_2of7.zip
|   +--- OpenJDK11U-jdk_x64_linux_hotspot_11.0.15_10.tar.gz
|   +--- ords-22.1.0.105.1723.zip
|   +--- put_software_here.txt
|   +--- sqlcl-22.1.1.131.0820.zip
+--- Vagrantfile
$
```