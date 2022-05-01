#tag homedrv/homeboot-images

FROM cr.shanhu.io/base/app
LABEL io.homedrive.name=homeboot

COPY shanhu.io/homedrv/drv/cmd/homeboot /opt/app/bin/homeboot
RUN ln -s /opt/app/bin/homeboot /bin/homeboot

CMD ["./bin/homeboot"]
