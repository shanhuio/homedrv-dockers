#tag cr.homedrive.io/homedrv/core
#in //go/shanhu.io/homedrv/daemon/jarvisd
#inzip //npm/jarvis/jarvis.zip

FROM cr.shanhu.io/base/alpine
LABEL io.homedrive.name=jarvis

RUN mkdir -p /opt/jarvis
RUN cd /opt/jarvis && mkdir bin var etc lib tmp

COPY jarvisd /opt/jarvis/bin/jarvisd
RUN ln -s /opt/jarvis/bin/jarvisd /bin/jarvisd
RUN ln -s /opt/jarvis/bin/jarvisd /bin/jarvis
RUN ln -s /opt/jarvis /opt/app

COPY lib /opt/jarvis/lib

WORKDIR /opt/jarvis
EXPOSE 3377

CMD ["./bin/jarvisd", "-addr=:3377"]
