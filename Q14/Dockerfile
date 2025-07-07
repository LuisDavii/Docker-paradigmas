
FROM ubuntu:22.04

RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    rm -rf /var/lib/apt/lists/*

RUN pip3 install pandas

COPY process.py /app/process.py

WORKDIR /app

CMD ["python3", "process.py"]