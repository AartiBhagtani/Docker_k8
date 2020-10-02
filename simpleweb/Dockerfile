# Specify base image
FROM node:alpine

# change working dir
WORKDIR /home/app

# install dependencies
COPY ./package.json ./
RUN npm install
COPY ./ ./

# default command
CMD ["npm", "start"] 