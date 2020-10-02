# use existing docker image as base image
From alpine
# Download and install dependency
RUN apk add --update redis
RUN apk add --update gcc
# Tell  image what to do when it starts as a container
CMD ["redis-server"]