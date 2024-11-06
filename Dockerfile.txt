FROM node:19-alpine #base image 

COPY package.json /app/
COPY src.js /app/

WORKDIR /app

RUN npm install 

CMD ["node","src.js"]
