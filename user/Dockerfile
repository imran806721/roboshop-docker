FROM node:20
WORKDIR /app
COPY package.json .
COPY *.js .
# node_modules
RUN npm install
ENV MONGO= "true" \
    MONGO_URL="mongodb://mongodb:27017/users"
CMD ["node", "server.js"]    