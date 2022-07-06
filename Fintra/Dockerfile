# base image
FROM node:14.19.1

# set working directory
WORKDIR /app

# install and cache app dependencies
# COPY package.json /app/package.json

# Use wildcard to install all of depandancies
COPY package*.json ./

RUN npm install
# RUN npm install -g @angular/cli@7.3.10

# add app
COPY . .

# EXPOSE port
EXPOSE 8080

# start app
CMD ["npm", "start"]