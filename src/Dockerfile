# Use a Node.js base image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json first to leverage Docker caching
COPY src/package.json . 

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY src/ .

# Expose port
EXPOSE 3000

# Command to run the app
CMD ["node", "index.js"]
