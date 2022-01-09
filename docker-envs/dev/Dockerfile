FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y vim git curl wget

RUN wget https://nodejs.org/dist/v16.13.1/node-v16.13.1-linux-x64.tar.xz
RUN tar -xf node-v16.13.1-linux-x64.tar.xz
RUN mv node-v16.13.1-linux-x64 /opt/
RUN echo "export NODEJS_HOME=/opt/node-v16.13.1-linux-x64/bin" >> ~/.bashrc
RUN echo "export PATH=$NODEJS_HOME:$PATH" >> ~/.bashrc

CMD ["tail", "-f", "/dev/null"]
