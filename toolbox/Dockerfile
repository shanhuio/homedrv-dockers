#tag cr.homedrive.io/homedrv/toolbox

FROM cr.shanhu.io/lib/base
LABEL io.homedrive.name=toolbox

RUN mkdir -p /opt/app
RUN cd /opt/app && mkdir bin var etc lib tmp

COPY shanhu.io/homedrv/drv/daemon/toolboxd /opt/app/bin/toolboxd
WORKDIR /opt/app

CMD ["./bin/toolboxd"]
