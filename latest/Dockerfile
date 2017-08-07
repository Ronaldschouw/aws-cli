FROM alpine:3.6

RUN apk update && \
		apk add python py-pip ca-certificates groff less && \
		rm -rf /var/cache/apk/* && \
		pip install awscli==1.11.129

ADD config /root/.aws/config

ENTRYPOINT ["aws"]
