FROM java:openjdk-8-jdk-alpine

MAINTAINER timzaak<zsy.evan@gmail.com>

ADD proxy-server-0.1 /proxy-server

RUN  apk add --no-cache bash && chmod a+x /proxy-server/bin/startup.sh && chmod a+x /proxy-server/bin/stop.sh

WORKDIR /proxy-server

ENTRYPOINT ["./bin/startup.sh"]