#tag cr.homedrive.io/ncfront
#in //go/shanhu.io/homedrv/daemon/ncfrontd

FROM cr.shanhu.io/base/alpine
MAINTAINER Shanhu Tech Inc.
LABEL io.homedrive.name=ncfront

RUN adduser -D ncfront -u 3000
COPY ncfrontd /bin/ncfrontd
RUN mkdir /opt/ncfront && chown ncfront /opt/ncfront

USER ncfront
WORKDIR /opt/ncfront
EXPOSE 8080
CMD ["/bin/ncfrontd"]
