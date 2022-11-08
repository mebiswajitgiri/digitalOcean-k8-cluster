FROM node:14-alpine

WORKDIR /app
RUN mkdir tasks \
    && touch ./tasks/tasks.txt
COPY package.json .

RUN npm install

COPY . .

EXPOSE 8000

CMD [ "node", "tasks-app.js" ]