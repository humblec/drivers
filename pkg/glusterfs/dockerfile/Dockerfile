FROM centos:7.4.1708

# Copy glusterfsplugin from build _output directory
COPY glusterfsplugin /glusterfsplugin

RUN yum -y install glusterfs-fuse && yum -y install epel-release && yum -y install jq && yum clean all

RUN rm -rf /var/cache/yum

ENTRYPOINT ["/glusterfsplugin"]
