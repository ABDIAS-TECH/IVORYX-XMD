FROM node:lts-buster
RUN git clone https://github.com/ABDIAS-TECH/IVORYX-XMD/root/ABDIAS-TECH
WORKDIR /root/ABDIAS-TECH
RUN npm install && npm install -g pm2 || yarn install --network-concurrency 1
COPY . .
EXPOSE 9090
CMD ["npm", "start"]
