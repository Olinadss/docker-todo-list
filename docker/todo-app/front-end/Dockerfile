FROM node:14-alpine
WORKDIR /docker/todo-app/front-end
COPY  package*.json ./
COPY node_modules.tar.gz ./
RUN npm install
EXPOSE 3000
COPY . .
ENV NODE_ENV=production
ENTRYPOINT [ "npm start" ]
