# Use an official Node.js runtime as a parent image
FROM node:12-alpine

# Set the working directory in the container
WORKDIR /result

# Copy package.json and package-lock.json
COPY package.json ./

# Install any needed packages specified in package.json
RUN npm install

# Bundle app source
COPY . .

# Expose port 80
EXPOSE 80

# Define command to run the app
CMD ["npm", "start"]
