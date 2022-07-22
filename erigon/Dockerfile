ARG UPSTREAM_VERSION

FROM thorax/erigon:${UPSTREAM_VERSION}

USER root

COPY entrypoint.sh /usr/bin/entrypoint.sh
RUN chmod u+x /usr/bin/entrypoint.sh
COPY jwt.hex /jwtsecret

ENTRYPOINT [ "/usr/bin/entrypoint.sh" ]
