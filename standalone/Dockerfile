FROM python:3.9-slim

RUN apt-get update && apt-get install -y \
    libffi-dev \
    libgmp-dev \
    libmpfr-dev \
    libmpc-dev \
    build-essential \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app
COPY . .

RUN pip install --upgrade pip \
 && pip install -r requirements.txt
