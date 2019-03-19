FROM node:8

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY content-init/package.json /usr/src/app/
RUN npm install

# Bundle app source
COPY content-init /usr/src/app

CMD [ "npm", "start" ]
