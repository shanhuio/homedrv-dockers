#tag cr.homedrive.io/homedrv/core
#in //go/shanhu.io/homedrv/daemon/jarvisd
#inzip //npm/jarvis/jarvis.zip

FROM cr.shanhu.io/base/app
LABEL io.homedrive.name=core

COPY jarvisd /opt/app/bin/jarvisd
RUN ln -s /opt/app/bin/jarvisd /bin/jarvisd
RUN ln -s /opt/app/bin/jarvisd /bin/jarvis

# TODO(h8liu): copy to lib directory
COPY _ /opt/app/_

WORKDIR /opt/app
EXPOSE 3377

CMD ["./bin/jarvisd", "-addr=:3377"]
