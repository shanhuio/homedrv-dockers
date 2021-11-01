#tag cr.homedrive.io/homedrv/toolbox
#in //go/shanhu.io/homedrv/daemon/toolboxd

FROM cr.shanhu.io/base/alpine
LABEL io.homedrive.name=toolbox

RUN mkdir -p /opt/app
RUN cd /opt/app && mkdir bin var etc lib tmp

COPY toolboxd /opt/app/bin/toolboxd
WORKDIR /opt/app

CMD ["./bin/toolboxd"]
