FROM golang:1.13.5-alpine3.11
RUN mkdir -p /var/go/test
ADD main.go /var/go/test/
RUN cd /var/go/test && go build
user root
EXPOSE 9090
WORKDIR /var/go/test/

ENTRYPOINT ["./main","--port","9090"]
