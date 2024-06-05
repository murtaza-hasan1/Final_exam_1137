# Use an official Node runtime as a parent image
FROM node:14

# Set the working directory
WORKDIR /usr/src/app/1137_backend

# Copy package.json and possibly package-lock.json
COPY package*.json ./

# Install any needed packages
RUN npm install

# Bundle app source
COPY . .

# Make port 1138 available to the world outside this container
EXPOSE 1140

# Command to run the app
CMD ["node", "index.js"]
