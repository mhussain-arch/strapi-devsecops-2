FROM python:3-alpine AS sqlmap

# Install Git to clone the SQLMap repo
RUN apk add --no-cache git

# Clone SQLMap into the image
RUN git clone --depth 1 https://github.com/sqlmapproject/sqlmap.git

# Set working directory
WORKDIR /sqlmap

# Ensure entrypoint runs SQLMap with Python 3
ENTRYPOINT ["python3", "sqlmap.py"]