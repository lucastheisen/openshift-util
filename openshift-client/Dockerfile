FROM centos:7

RUN yum install -y centos-release-scl && \
    yum install -y centos-release-openshift-origin36 && \
    INSTALL_PACKAGES=" \
    docker-client \
    origin-clients \
    " && \
    yum install -y --setopt=tsflags=nodocs $INSTALL_PACKAGES && \
    rpm -V $INSTALL_PACKAGES && \
    yum clean all -y

CMD ["/bin/bash"]
