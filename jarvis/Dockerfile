#tag cr.homedrive.io/core
#in //go/shanhu.io/homedrv/daemon/jarvisd
#inzip //npm/jarvis/jarvis.zip

FROM cr.shanhu.io/base/alpine
MAINTAINER Shanhu Tech Inc.
LABEL io.homedrive.name=jarvis

COPY jarvisd /bin/jarvisd
RUN ln -s /bin/jarvisd /bin/jarvis
RUN mkdir /opt/jarvis
COPY _ /opt/jarvis/_
WORKDIR /opt/jarvis
EXPOSE 8080
CMD ["/bin/jarvisd", "-addr=:3377"]
