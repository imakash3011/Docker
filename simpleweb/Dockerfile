# Specify a base image
FROM node:alpine
# adding following line because newser version of node throw error of "idealtree exist"
WORKDIR /usr/app

# copying package.json to Current dir. of container to avoid installation of all 
# dependencies again and again
COPY ./package.json ./
# Install some dependencies
RUN npm install
# copying content from current directory to Current dir. of container
COPY ./ ./

# Default command
CMD [ "npm","start"]