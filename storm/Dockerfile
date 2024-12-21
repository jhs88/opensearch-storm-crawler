ARG STORM_VERSION=2.6.4
FROM storm:${STORM_VERSION} AS base
COPY conf/storm.yaml /conf/storm.yaml

FROM base AS runner
ENV JAVA_HOME=/usr/lib/jvm/default-java
RUN apt update; \
    apt install -y maven software-properties-common; \
    apt autoremove && apt clean;
USER storm
