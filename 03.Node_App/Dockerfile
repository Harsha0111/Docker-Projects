# Use the official Node.js image with version 18 (alpine variant)
FROM node:18-slim

# Set working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all other source code to the working directory
COPY . .

# Specify the command to run your Node.js application
CMD ["node", "index.js"]

# Expose port 3001
EXPOSE 3001
