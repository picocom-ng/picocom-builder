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
		libconfuse \
		libconfuse-devel \
		cmake \
		libffi-devel \
		libgit2-devel \
		check \
		check-devel \
		gcovr \
		bats && \
	yum clean all

ENV LD_LIBRARY_PATH=/usr/local/lib64:/usr/local/lib
