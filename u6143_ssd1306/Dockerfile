ARG BUILD_FROM
FROM ${BUILD_FROM}

# Copy root filesystem
COPY rootfs /

# Setup base
RUN apk add --no-cache \
    procps \
 && apk add --no-cache --virtual .build-dependencies \
    build-base \
    git \
    linux-headers

RUN git clone https://github.com/darkgrue/U6143_ssd1306.git \
 && cd /U6143_ssd1306/C \
 && make \
 && cp display /usr/local/bin/ \
 && apk del .build-dependencies \
 && cd / \
 && rm -rf /U6143_ssd1306