FROM node:8

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY content-web-v2/package.json /usr/src/app/
RUN npm install

# Bundle app source
COPY content-web-v2 /usr/src/app

EXPOSE 3000
CMD [ "npm", "start" ]
