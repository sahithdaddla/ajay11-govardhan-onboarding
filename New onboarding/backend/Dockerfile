# Use official Node.js LTS image
FROM node:18-alpine

# Create app directory
WORKDIR /app

# Copy package.json and package-lock.json first (for caching install step)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port your app runs on (from server.js, likely 3000)
EXPOSE 3420

# Start the application
CMD ["node", "server.js"]

