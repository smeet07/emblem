FROM --platform=linux/amd64 node:19.8.1 as client-app-build

USER root
WORKDIR /usr/src/app
COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 8000

CMD ["npm", "run", "start"]
