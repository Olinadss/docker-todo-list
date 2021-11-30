FROM mjgargani/puppeteer:trybe1.0
WORKDIR /docker/todo-app/tests
COPY  package*.json ./
ADD node_modules.tar.gz ./
RUN npm install
COPY . .
ENV FRONT_HOST=localhost
ENV FRONT_PORT=3000
ENTRYPOINT [ "npm test" ]