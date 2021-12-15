ARG PLATFORM=amd64
ARG DISTRIBUTION=alpine
ARG VARIANT=latest
FROM --platform="$PLATFORM" "$DISTRIBUTION":"$VARIANT"

ARG PLATFORM=${PLATFORM:-amd64}
ARG S6_OVERLAY_VERSION=v2.2.0.3

LABEL maintainer="Jesse N. <jesse@keplerdev.com" \
      org.opencontainers.image.author="Jesse N. <jesse@keplerdev.com>" \
      org.opencontainers.image.source="https://github.com/jessenich/docker-s6-overlay"

ADD https://github.com/just-containers/s6-overlay/releases/download/$S6_OVERLAY_VERSION/s6-overlay-$PLATFORM.tar.gz /tmp/s6-overlay-$PLATFORM.tar.gz
RUN tar xvzf /tmp/s6-overlay-$PLATFORM.tar.gz -C /

