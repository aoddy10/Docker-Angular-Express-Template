FROM node:12
  
# Create a directory where our app will be placed
RUN mkdir -p /usr/src/app

# Change directory so that our commands run inside this new directory
WORKDIR /usr/src/app

# Get all the code needed to run the app
COPY . .

# Install dependecies
RUN npm install

RUN npm install -g @angular/cli@8.3.12

RUN npm build

# Expose the port the app runs in
# EXPOSE 4200