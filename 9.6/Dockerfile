FROM postgres:9.6

ENV POSTGIS_VERSION=2.3

RUN apt-get update \
  && DEBIAN_FRONTEND=noninteractive apt-get install --no-install-recommends -y \
    postgresql-$PG_MAJOR-postgis-$POSTGIS_VERSION \
    postgresql-$PG_MAJOR-postgis-$POSTGIS_VERSION-scripts \
    postgresql-contrib-$PG_MAJOR \
    postgresql-$PG_MAJOR-pgrouting \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*
