FROM bde2020/hadoop-base:1.0.0
MAINTAINER Ivan Ermilov <ivan.s.ermilov@gmail.com>

ENV HDFS_CONF_dfs_datanode_data_dir=file:///hadoop/dfs/data
RUN mkdir -p /hadoop/dfs/data
VOLUME /hadoop/dfs/data

ADD run.sh /run.sh
RUN chmod a+x /run.sh

EXPOSE 50075

CMD ["/run.sh"]
