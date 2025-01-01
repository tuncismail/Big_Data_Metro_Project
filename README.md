# Big_data_metro_project
2024-2025 Big Data Project


# go and take the data from https://data.ibb.gov.tr/dataset/hourly-public-transport-data-set
take first 6-12 months from 2023 


# install kafka to ubuntu wsl
    run kafka and zookeeper run publisher function with formetted data
    consumer will show consuemd data in list of dictonaries







# Hbase installation

https://hub.docker.com/r/dajobe/hbase/

install hbase image
run it with given ports

run the container look at ports with 
in cmd docker ps

 see for port:9090 the port written in ”port” is your port




docker image running:
when run image use given ports in right hand side and for paths set C:\docker\hbase\data in left and /data in right

configuration:
after running container of hbase go ubuntu kafka files and find server.properities and zookeeper.properities change port to 2083 for zookeeper and for server.properities change kafka listener port to 2083 
 


# unnecessary
Port Mapping: If you want to access HBase’s web UIs or Thrift/REST APIs from your host machine, you need to “Publish a port.” For each port:
Click “Publish a port” (or “Add port”).
Set the container port to 16010 for the HBase Master UI, 16030 for RegionServer UI, 9090 for Thrift, 8080 for REST, etc.
Set the host port to the same or a different number if there’s a conflict. For example, 16010 on host → 16010 in container.
Volumes: If you want to persist data to your local drive so that it’s not lost when the container is removed, mount a volume:
Under “Volumes” (or “Mounts”), choose “Bind” or “Host path”.
Select a path on your Windows host (e.g., C:\docker\hbase\data) and map it to the container path /data.





# load to hbase use chatgpt
import happybase
conn = happybase.Connection(host='localhost', port=9089)
conn.create_table('test', {'cf': dict()})
print(conn.tables())       







# load to hbase
load data to hbase after consuming from consumer you can run consumer,publisher and happybase in both your windows or ubuntu wsl


# with query codes take data rom hbase and data_to_model converter for last 1 hour data you should make some changes to do that
# predict the next hour customers with model
# save the prediction we may do geospatial plot it is based on ismail's position