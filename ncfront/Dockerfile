#tag cr.homedrive.io/homedrv/ncfront
#in //go/shanhu.io/homedrv/daemon/ncfrontd

FROM cr.shanhu.io/base/alpine
MAINTAINER Shanhu Tech Inc.
LABEL io.homedrive.name=ncfront

RUN adduser -D -u 3000 app
RUN mkdir -p /opt/app
RUN cd /opt/app && mkdir bin var etc lib tmp
RUN chown -R app /opt/app
WORKDIR /opt/app

COPY ncfrontd /opt/app/bin/ncfrontd
EXPOSE 8080

USER app

CMD ["./bin/ncfrontd"]
