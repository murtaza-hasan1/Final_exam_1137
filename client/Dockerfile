# Use an official Node runtime as a parent image
FROM node:14

# Set the working directory
WORKDIR /usr/src/app/1137_frontend

# Copy package.json and possibly package-lock.json
COPY package*.json ./

# Install any needed packages
RUN npm install

# Bundle app source
COPY . .

# Build the application
RUN npm run build

# Install serve to serve the application
RUN npm install -g serve

# Make port 1137 available to the world outside this container
EXPOSE 1137

# Command to run the app
CMD ["serve", "-s", "build", "-l", "1137"]
