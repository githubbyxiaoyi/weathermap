#FROM openjdk:8u181-jdk-alpine
FROM swr.cn-north-1.myhuaweicloud.com/codeci/special_base_image:centos7-base-1.0.2
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
    echo "Asia/Shanghai" > /etc/timezone

WORKDIR /home/apps/
ADD target/weather-beta-2.0.0.jar .
ADD start.sh .

ENTRYPOINT ["sh", "/home/apps/start.sh"]
