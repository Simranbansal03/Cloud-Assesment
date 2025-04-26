# Use official Node.js v14 image
FROM node:14

# Set working directory
WORKDIR /app

# Copy package.json first (for caching install layer)
COPY package.json .

# Install dependencies (none for now, but required step)
RUN npm install

# Copy app code
COPY . .

# Expose the app port
EXPOSE 3000

# Start the app
CMD ["npm", "start"]