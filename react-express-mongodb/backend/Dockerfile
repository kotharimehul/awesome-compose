FROM node:lts-buster-slim

# Create app directory
WORKDIR /usr/src/app

# COpy package files to cointainer
COPY package.json /usr/src/app/package.json
COPY package-lock.json /usr/src/app/package-lock.json

#Install Dependencies
RUN npm ci

# Copy all code for app
COPY . /usr/src/app


# Expose the port
EXPOSE 3000

# STart the server
CMD [ "npm", "run", "dev" ]
