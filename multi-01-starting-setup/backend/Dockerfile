FROM node
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
ENV MONGODB_USERNAME=ajith
ENV MONGODB_PWD=secret
EXPOSE 80
CMD [ "npm" , "start" ]