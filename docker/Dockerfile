FROM gliderlabs/logspout:v3.2.3
ENV SYSLOG_FORMAT rfc3164

RUN apk update && apk upgrade  # separate security updates are not available, so updating all packages

ADD ./entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
