docker-mesos
=====

A simple distributed computing cluster-in-a-box: Mesos, zookeeper, marathon. 

Use other physical computers to add computational power to the cluster.


###Use:
* Clone repository
* ./build.sh
* fig up -d

The mesos-master default port of 5050 has been left to be tied to any random port on the host (This can be changed by replacing 5050 with 15050:5050 for eg. in fig.yml)

However, doing so allows you to change the quorum inside the mesos-master/Dockerfile and scale up the mesos-masters using 
* fig scale master=<3 or 5 or whatever>

To open up the Mesos UI, open http://your docker host's IP:15050
in case you tie the mesos-master to 15050 (you can only have a single master then)
or determine the port used on the host by doing a 
sudo docker ps | grep dockermesos_master

To open up 
Marathon UI: open http://your docker host's IP:10080


```
