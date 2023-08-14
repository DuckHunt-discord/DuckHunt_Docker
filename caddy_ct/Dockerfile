FROM caddy:2.7.3-builder AS builder

RUN xcaddy build \
    --with github.com/caddyserver/transform-encoder

FROM caddy:2

COPY --from=builder /usr/bin/caddy /usr/bin/caddy