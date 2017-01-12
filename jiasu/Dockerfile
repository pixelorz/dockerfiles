FROM alpine:latest

RUN set -ex \
	&& apk add --no-cache libsodium py2-pip \
    && pip --no-cache-dir install https://github.com/shadowsocks/shadowsocks/archive/master.zip
#ADD config.json /config.json
#EXPOSE your_port	
ENTRYPOINT ["/usr/bin/ssserver"]
# usage:
# docker run -d --restart=always -p 443:443 index.docker.io/user/project:tag -s 0.0.0.0 -p 443 -k $PD -m chacha20
