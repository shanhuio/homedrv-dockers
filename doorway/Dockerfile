#tag cr.homedrive.io/homedrv/doorway
#in //go/shanhu.io/homedrv/daemon/doorwayd

FROM cr.shanhu.io/base/alpine
MAINTAINER Shanhu Tech Inc.
LABEL io.homedrive.name=doorway

RUN adduser -D -u 3000 app
RUN mkdir -p /opt/app
RUN cd /opt/app && mkdir bin var etc lib tmp
RUN chown -R app /opt/app
WORKDIR /opt/app

COPY doorwayd /opt/app/bin/doorwayd
EXPOSE 8080
EXPOSE 8433

USER app

CMD ["./bin/doorwayd"]
