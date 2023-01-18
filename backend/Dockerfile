FROM node:17-alpine3.14
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD [ "node", "index.js", "todo-inmemory.js", "todo-mysql.js", "verify.js" ]
