#tag cr.homedrive.io/homedrv/ncfront
#in //go/shanhu.io/homedrv/daemon/ncfrontd

FROM cr.shanhu.io/base/app
LABEL io.homedrive.name=ncfront

COPY ncfrontd /opt/app/bin/ncfrontd
EXPOSE 8080

USER app

CMD ["./bin/ncfrontd"]
