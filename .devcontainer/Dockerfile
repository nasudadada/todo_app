FROM mcr.microsoft.com/vscode/devcontainers/python:0-3.9

RUN apt-get update && apt-get install -y nodejs npm
RUN npm install -g n && n stable

WORKDIR /workspace

COPY backend/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

RUN npm install -g next