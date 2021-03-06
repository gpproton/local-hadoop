# Local Hadoop Cluster
This project creates a small local Hadoop cluster using [Cloudera Manager 6.3.0](https://www.cloudera.com/downloads/manager/6-3-0.html) on a [CentOS 7.6](http://isoredirect.centos.org/centos/7/isos/x86_64/CentOS-7-x86_64-DVD-1810.iso) base.

![Server Architecture Diagram](images/server-architecture.svg)

## Installation Steps
1. Create the [Base CentOS](https://github.com/JohnnyFoulds/local-hadoop/wiki/Base-Virtual-Machine) virtual machine.
2. Create the [Base Manager](https://github.com/JohnnyFoulds/local-hadoop/wiki/Manager-Base) virtual machine.
3. Create the [Worked Nodes](https://github.com/JohnnyFoulds/local-hadoop/wiki/Worker-Nodes).
4. [Download and Run](https://github.com/JohnnyFoulds/local-hadoop/wiki/Cloudera-Manager-Install) the Cloudera Manager Server Installer.
5. Navigate to `http://192.168.3.200:7180` and login in with `admin`, `admin`.
6. Follow the installation wizard and use the `hadoop-manager.lan, hadoop-worker[01-03].lan` pattern when adding hosts.

## Pages of Interest
- [vSphere](https://github.com/JohnnyFoulds/local-hadoop/wiki/vSphere) - This shows how the server configuration was done on the physical hardware.
- [vCenter](https://github.com/JohnnyFoulds/local-hadoop/wiki/vCenter) - The vCenter Installation which was a bit finicky at times.
- [PowerCLI](https://github.com/JohnnyFoulds/local-hadoop/wiki/PowerCLI) - Some helpful reference examples on the essentials of using VMWare PowerCLI.
- [vnc](https://github.com/JohnnyFoulds/local-hadoop/wiki/vnc) - Well not really, the better alternative to VNC when you are using VMWare.

## Web References
- Installation Path A - Automated Installation by Cloudera Manager - https://www.cloudera.com/documentation/enterprise/5-6-x/topics/cm_ig_install_path_a.html
- Installing a Proof-of-Concept Cluster - https://www.cloudera.com/documentation/enterprise/6/6.3/topics/cm_ig_non_production.html