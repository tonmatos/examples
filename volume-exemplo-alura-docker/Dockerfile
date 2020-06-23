## image:version
FROM node:latest
## Name of who is maintaining this image
MAINTAINER Wanilton Filho
## Expose env variables
ENV NODE_ENV=production
ENV PORT=3000
## FROM TO
COPY . /var/www
## Directory where the files are. Load the project in this directory and execute commands
WORKDIR /var/www
## Execute a command when image is being built. (npm install download all dependencies)
RUN npm install
## Command to be execute after the container starts.
ENTRYPOINT ["npm", "start"]
## Exposed port
EXPOSE $PORT
