FROM node:18.16.1

WORKDIR /usr/src/app

COPY . .

RUN npm install
RUN apt update && \
    apt install -y wget netcat-openbsd && \
    wget -q -O /usr/bin/wait-for https://raw.githubusercontent.com/eficode/wait-for/v2.2.3/wait-for && \
    chmod +x /usr/bin/wait-for

EXPOSE 3000
