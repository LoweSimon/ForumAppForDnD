FROM node:10.16-alpine

# Create App Directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# install dependencies
COPY package*.json ./

RUN npm install --silent

# copy app source code
COPY . .

# exports
EXPOSE 4000

CMD ["npm","start"]