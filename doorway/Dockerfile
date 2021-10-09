#tag cr.homedrive.io/homedrv/doorway
#in //go/shanhu.io/homedrv/daemon/doorwayd

FROM cr.shanhu.io/base/app
LABEL io.homedrive.name=doorway

COPY doorwayd /opt/app/bin/doorwayd
EXPOSE 8080
EXPOSE 8433

USER app

CMD ["./bin/doorwayd"]
