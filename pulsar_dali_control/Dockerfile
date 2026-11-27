FROM ghcr.io/home-assistant/base:latest

ARG BUILD_VERSION
ARG BUILD_ARCH

RUN apk add --no-cache python3 py3-pyserial py3-smbus openssl

COPY run.sh /
COPY app /tmp/pulsar_app
RUN mkdir -p /app     && cat /tmp/pulsar_app/pulsar_dali_control.py.gz.b64.* | base64 -d | gzip -d > /app/pulsar_dali_control.py     && rm -rf /tmp/pulsar_app     && chmod a+x /run.sh

LABEL   io.hass.version="$BUILD_VERSION"   io.hass.type="app"   io.hass.arch="$BUILD_ARCH"

CMD [ "/run.sh" ]
