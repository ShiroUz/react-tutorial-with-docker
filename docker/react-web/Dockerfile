FROM node:20.4.0-bullseye-slim

RUN mkdir /app && chown node:node /app
WORKDIR /app

USER node

COPY --chown=node:node react-tutorial-with-docker-impl/package.json react-tutorial-with-docker-impl/package-lock.json ./

RUN npm install

COPY --chown=node:node react-tutorial-with-docker-impl ./

EXPOSE 3000

CMD [ "npm", "start" ]
