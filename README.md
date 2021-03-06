# Ambari-Elastic-Service11111111111111111111

## Project
### Elasticsearch 6.4.x
|  Feature   |  Description       |
| -----------| -----------------|
| Version | 6.4.2 |
| Service | Elasticsearch |
| Component-Master | Elasticsearch-Master (node.master=true, node.data=true) |
| Component-Slave | Elasticsearch-Slave (node.master=flase, node.data=true)  |
| Extra | Including all X-Pack features |

### Kibana 6.4.x
|  Feature   |  Description       |
| -----------| -----------------|
| Version | 6.4.2 |
| Service | Kibana |
| Component-Master | Kibana-Sever |
| Extra | Including all X-Pack features |


## Prerequisite
|  Software   |  Version | Status  |
| -----------| -----------------| -----------------|
| Ambari | 2.x (test on 2.6.2.0) | Fully Installed |


## How to use
1. Download the source code.
2. Copy the project folder to ambari 's lib folder. Such as:
```
cp -r ./ELASTICSEARCH-6.4.x /var/lib/ambari-server/resources/stacks/HDP/2.6/services
```
3. Restart ambari-server:
```
ambari-server restart
```
4. Log into web then add service as usual. Such as:
![image](https://github.com/BalaBalaYi/Ambari-Elastic-Service/blob/master/doc/es-ambari-1.png)

5. Choose node.

6. Configure the service.
#### Elasticsearch
![config](/doc/es-ambari-2.png)
![config](/doc/es-ambari-3.png)

#### Kibana
![config](/doc/kibana-ambari-1.png)
![config](/doc/kibana-ambari-2.png)

7. Finish the installation then enjoy urself.^^


## Notice
1. Can be used in non-internet environment. But need to install all the dependency packages and upload the installation packages to the private-repo before the installation.
2. Need more test if using on production.
