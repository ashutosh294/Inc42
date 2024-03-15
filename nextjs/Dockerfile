# Use an official Node.js image as a parent image
FROM node:14-alpine

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the local source files to the container
COPY . .

# Build the Next.js application
RUN npm run build

# Expose the port on which the service will run
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]
