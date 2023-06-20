FROM postgres:11-alpine AS deploy
RUN apk add binutils make libgcc musl-dev gcc linux-headers

WORKDIR /opt
RUN wget -O pgaudit.tar.gz https://github.com/pgaudit/pgaudit/archive/refs/tags/1.3.4.tar.gz
RUN ls -l pgaudit.tar.gz
RUN tar -xzf pgaudit.tar.gz && rm pgaudit.tar.gz

WORKDIR /opt/pgaudit-1.3.4
RUN make install USE_PGXS=1 PG_CONFIG=/usr/local/bin/pg_config

RUN apk del binutils make gcc