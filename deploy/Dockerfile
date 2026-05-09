FROM eclipse-temurin:11-jre-focal

MAINTAINER 阿沐

# 设置时区
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo 'Asia/Shanghai' >/etc/timezone

WORKDIR /app

# 【关键修改】复制具体的 jar 包名称
COPY maku-server.jar /app/maku-server.jar

ENTRYPOINT ["java", \
            "-server", \
            "-Xms256m", \
            "-Xmx512m", \
            "-Djava.security.egd=file:/dev/./urandom", \
            "-Dfile.encoding=UTF-8", \
            "-jar", "/app/maku-server.jar" ]
