#tag cr.homedrive.io/doorway
#in //go/shanhu.io/homedrv/daemon/doorwayd

FROM cr.shanhu.io/base/alpine
MAINTAINER Shanhu Tech Inc.
LABEL io.homedrive.name=doorway

RUN adduser -D -u 3000 doorway
COPY doorwayd /bin/doorwayd
RUN mkdir -p /etc/homedrv/doorway && chown doorway /etc/homedrv/doorway
RUN mkdir -p /var/lib/homedrv/doorway && chown doorway /var/lib/homedrv/doorway

USER doorway
WORKDIR /
EXPOSE 8080
EXPOSE 8433
CMD ["/bin/doorwayd"]
