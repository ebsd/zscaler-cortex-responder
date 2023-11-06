FROM python:3

WORKDIR /worker
COPY . Zscaler

RUN test ! -e Zscaler/requirements.txt || pip install --no-cache-dir -rZscaler/requirements.txt

ENTRYPOINT Zscaler/zscaler.py
