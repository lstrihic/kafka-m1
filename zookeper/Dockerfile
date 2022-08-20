FROM arm64v8/openjdk:18.0.2.1-jdk
WORKDIR /app
RUN /bin/curl https://dlcdn.apache.org/kafka/3.2.1/kafka_2.13-3.2.1.tgz --output kafka_2.13-3.2.1.tgz --silent
RUN /bin/tar -xf kafka_2.13-3.2.1.tgz
WORKDIR /app/kafka_2.13-3.2.1
CMD ["bin/zookeeper-server-start.sh", "config/zookeeper.properties"]