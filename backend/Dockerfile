FROM node

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=mongoadmin

ENV MONGODB_PASSWORD=secret

CMD ["npm", "run", "dev"]
