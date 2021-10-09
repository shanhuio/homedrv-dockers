#tag homedrv/homeboot-images
#tag cr.homedrive.io/homedrv/homeboot
#in //go/shanhu.io/homedrv/cmd/homeboot

FROM cr.shanhu.io/base/app
LABEL io.homedrive.name=homeboot

COPY homeboot /opt/app/bin/homeboot
RUN ln -s /opt/app/bin/homeboot /bin/homeboot

CMD ["./bin/homeboot"]
