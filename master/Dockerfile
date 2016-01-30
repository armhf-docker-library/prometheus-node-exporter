FROM armhfbuild/golang:1.5.3

RUN mkdir /build \
  && cd /build \
  && git clone https://github.com/prometheus/node_exporter.git . \
  && make \
  && cp ./node_exporter /usr/local/bin/

EXPOSE 9100
CMD ["node_exporter"]
