FROM docker:cli
LABEL maintainer="Lukas Korl <hello@lukaskorl.com>"

RUN apk add --no-cache curl git jq ca-certificates envsubst yq apache2-utils bash && \
    rm -rf /var/cache/apk/* && \
    mkdir -p ~/.ssh && \
    chmod 700 ~/.ssh
