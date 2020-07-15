# Banking Insurance
This project is to track and identify the creditcard defaulters and define the insurance premium
according to the list of defaulters by joining data from insurance system, creditcard systems, state
code fixed width data and the customer master datasets. 
## Getting Started
 - Install VMware 15 player 
 - Install centos
 - Install requirements
 - Start Services
 - Run the scripts
## Local Installation
**Install the requirements:**
$ pip install -r Requirements.txt

**Make sure you have the following installed:**
- Hadoop
- Sqoop
- Hive
- Hbase
- Phoenix
- Zookeeper

**Installing mysql & postgresql**
- [Install mysql](https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-centos-7).
- [Install postgresql](https://linuxize.com/post/how-to-install-postgresql-on-centos-7/).
## Starting services 
- Start Hadoop
  - start-all.sh 
  - mr-jobhistory-daemon.sh start historyserver (job history server)
- Start mysql service
  - service mysqld start
- Start Hive metastore in a terminal
  - hive --service metastore & (as background service)
- Start Hbase
  - start-hbase.sh 
- Start Zookeeper
  - zkServer.sh start
- Start Phoenix
  - sqlline.py localhost
## Run the scripts
   Generate reports from the final table