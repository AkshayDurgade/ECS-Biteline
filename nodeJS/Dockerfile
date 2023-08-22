# To install this docker image use the following commands or refer the following link


# Using base image and OS as node alpine
FROM node:alpine

# Changing our working directory to the following path
WORKDIR /home/node-app/app

# Copying package files into the Image at once only. Not repeating it
COPY package*.json ./

# Installing all the dependencies 
RUN npm install

# Copying all the content inside of image 
COPY . .

# Exposing port No 3000 of the container for port mapping 
EXPOSE 3000

# Change the entry point file name depending upon the requirements
CMD ["node","index.js"]
