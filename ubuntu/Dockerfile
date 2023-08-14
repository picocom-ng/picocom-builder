ARG UBUNTU_VERSION=22.04
FROM ubuntu:${UBUNTU_VERSION}

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
	apt-get -y install \
		build-essential \
		gcc gcc-11 gcc-10 gcc-9 \
		gdb gdbserver \
		curl \
		less \
		libubsan1 \
		libasan8 \
		git \
		libconfuse2 \
		libconfuse-dev \
		cmake \
		libffi-dev \
		libgit2-dev \
		pkg-config \
		check \
		gcovr \
		bats \
		pandoc \
		htmldoc \
        && \
	apt-get clean
