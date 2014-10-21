FROM mesos
MAINTAINER akshshar 

EXPOSE 5050

CMD ["--zk=zk://zookeeper:2181/mesos", "--work_dir=/var/lib/mesos", "--quorum=2"]

ENTRYPOINT ["mesos-master"]
