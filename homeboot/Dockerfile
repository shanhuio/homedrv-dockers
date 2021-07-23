#tag homedrv/homeboot-images
#tag cr.homedrive.io/homeboot
#in //go/shanhu.io/homedrv/cmd/homeboot

FROM cr.shanhu.io/alpine
MAINTAINER Shanhu Tech Inc.
LABEL io.homedrive.name=homeboot

COPY homeboot /bin/homeboot
RUN mkdir /opt/homedrv
WORKDIR /opt/homedrv
CMD ["/bin/homeboot"]
