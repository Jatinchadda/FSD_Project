# Use official Node.js image
FROM node:20

# Set working directory inside container
WORKDIR /app

# Copy package.json and package-lock.json first (for better caching)
COPY package*.json ./

# Install all dependencies
RUN npm install

# Copy the rest of the source code
COPY . .

# Expose the app port
EXPOSE 8080

# Start the app
CMD ["npm", "start"]
