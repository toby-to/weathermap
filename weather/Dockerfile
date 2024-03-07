FROM openjdk:8u181-jdk-alpine

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone

WORKDIR /home/apps2/
ADD target/weather-1.0.0.jar .
ADD start.sh .

ENTRYPOINT ["sh", "/home/apps2/start.sh"]
