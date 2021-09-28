#tag homedrv/homeboot-images
#tag cr.homedrive.io/homedrv/homeboot
#in //go/shanhu.io/homedrv/cmd/homeboot

FROM cr.shanhu.io/base/alpine
MAINTAINER Shanhu Tech Inc.
LABEL io.homedrive.name=homeboot

RUN mkdir -p /opt/app
RUN cd /opt/app && mkdir bin var etc lib tmp
WORKDIR /opt/app

COPY homeboot /opt/app/bin/homeboot
RUN ln -s /opt/app/bin/homeboot /bin/homeboot
WORKDIR /opt/app

CMD ["./bin/homeboot"]
