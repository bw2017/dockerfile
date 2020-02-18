FROM centos:centos7
RUN yum install -y wget && mkdir /usr/local/node && cd /usr/local/node && wget https://npm.taobao.org/mirrors/node/v8.17.0/node-v8.17.0-linux-x64.tar.gz && tar zxf node-v8.17.0-linux-x64.tar.gz 
ENV NODE_HOME=/usr/local/node/node-v8.17.0-linux-x64
ENV PATH=$PATH:$NODE_HOME/bin NODE_PATH=$NODE_HOME/lib/node_modules
RUN $NODE_HOME/bin/npm install elasticdump -g --registry=http://registry.npm.taobao.org

