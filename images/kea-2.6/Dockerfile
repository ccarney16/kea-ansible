FROM almalinux:9

RUN \
    dnf install -y epel-release && \
    crb enable && \
    curl -1sLf 'https://dl.cloudsmith.io/public/isc/kea-2-6/setup.rpm.sh' | \
    bash && \
    dnf install -y isc-kea && \
    dnf clean all

USER kea:kea
