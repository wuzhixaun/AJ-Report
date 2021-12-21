FROM anapsix/alpine-java:8_server-jre_unlimited

MAINTAINER jackWu <wuzhixuano@qq.com>

RUN mkdir -p /blade/report

WORKDIR /blade/report

EXPOSE 80

ADD ./target/*.jar ./app.jar

ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "app.jar"]
