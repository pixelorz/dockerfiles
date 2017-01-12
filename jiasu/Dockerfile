FROM alpine:latest

RUN set -ex \
	&& apk add --no-cache libsodium py2-pip \
    && pip --no-cache-dir install https://github.com/shadowsocks/shadowsocks/archive/master.zip
#ADD config.json /config.json
#EXPOSE 1248	
ENTRYPOINT ["/usr/bin/ssserver"]
