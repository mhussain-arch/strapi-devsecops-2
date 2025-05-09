# .github/sqlmap/Dockerfile
FROM alpine:3.1

LABEL maintainer="Paolo Oliveira <paolo@fisica.ufc.br>"

RUN apk add --no-cache python git                  \
 && git clone https://github.com/sqlmapproject/sqlmap.git /sqlmap

WORKDIR /sqlmap
ENTRYPOINT ["python", "sqlmap.py"]