# Use official Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY src/package.json .
RUN npm install

# Copy application files
COPY src/ .

# Expose port
EXPOSE 3000

# Start application
CMD ["npm", "start"]
