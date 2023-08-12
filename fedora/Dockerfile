ARG FEDORA_VERSION=38
FROM quay.io/fedora/fedora:${FEDORA_VERSION}

RUN yum -y groupinstall c-development && \
	yum -y install \
		gdb gdb-gdbserver \
		curl \
		less \
		xz \
		libasan \
		libubsan \
		git \
		meson \
		ninja-build \
		libconfuse \
		libconfuse-devel \
		cmake \
		libffi-devel \
		libgit2-devel \
		bats && \
	yum clean all

COPY install-criterion.sh ./
RUN bash install-criterion.sh

ENV LD_LIBRARY_PATH=/usr/local/lib64:/usr/local/lib
