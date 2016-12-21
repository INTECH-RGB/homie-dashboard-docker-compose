FROM resin/armhf-alpine:3.4

RUN apk add --no-cache mosquitto

RUN mkdir -p /mosquitto/config /mosquitto/data
COPY mosquitto.conf /mosquitto/config
RUN chown -R mosquitto:mosquitto /mosquitto

VOLUME ["/mosquitto/config", "/mosquitto/data"]

EXPOSE 1883

CMD ["mosquitto", "-c", "/mosquitto/config/mosquitto.conf"]
