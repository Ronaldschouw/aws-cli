FROM alpine

RUN apk update && \
		apk add python3 py-pip ca-certificates groff less && \
		rm -rf /var/cache/apk/* && \
		pip install awscli

ADD keeprunning.sh /
CMD  /keeprunning.sh
