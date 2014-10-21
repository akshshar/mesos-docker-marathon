FROM mesos
MAINTAINER akshshar

CMD ["--master=zk://zookeeper:2181/mesos", "--log_dir=/var/log/mesos"]

ENTRYPOINT ["mesos-slave"]
