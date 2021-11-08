FROM ubuntu:20.04
MAINTAINER supperthomas <78900636@qq.com>
ARG DEST_DIR=/root

WORKDIR ${DEST_DIR}

RUN sed -i 's/http:\/\/archive.ubuntu.com\/ubuntu\//http:\/\/mirrors.aliyun.com\/ubuntu\//g' /etc/apt/sources.list && apt-get update


RUN apt-get update

RUN apt-get upgrade -y

RUN apt-get install -y git

RUN apt-get install -y python3 python-is-python3 

RUN apt-get install -y pip

RUN apt-get install -y scons

RUN apt-get install -y libncurses5-dev

RUN apt-get install -y vim

RUN pip install requests -qq

RUN apt-get install -y wget

RUN apt-get install -y gcc-arm-none-eabi

ENV RTT_EXEC_PATH=/usr/bin

#RUN git clone https://gitee.com/superThomas/rt-thread_github.git

WORKDIR /root/rt-thread

#RUN python -c "import tools.menuconfig; tools.menuconfig.touch_env()"

RUN apt-get clean

RUN rm -rf /var/lib/apt/lists/*
#not work
#RUN /bin/bash -c "source ~/.env/env.sh"
#RUN ["/bin/bash", "-c", "source ~/.env/env.sh"]
ENV RTT_CC=gcc


