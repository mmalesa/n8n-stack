FROM n8nio/runners:latest

USER root

RUN apt-get update && apt-get install -y \
    python3 python3-pip python3-venv \
    ca-certificates curl \
    poppler-utils \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install --no-cache-dir \
    yfinance \
    pandas \
    numpy \
    pdfplumber \
    pyarrow

USER node

