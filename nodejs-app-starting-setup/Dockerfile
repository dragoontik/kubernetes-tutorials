FROM node:17

WORKDIR /app

COPY package.json /app
# can also do COPY . ./

RUN npm install

COPY . /app

EXPOSE 80

# RUN node server.js - WRONG!!
CMD ["node", "server.js"]


