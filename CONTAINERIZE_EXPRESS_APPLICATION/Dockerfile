# Execution Sequence : 
# Load basic Image
# Set work directory
# Copy package jsons
# Install dependencies
# Copy the source code
# Expose the application port
# Start Application


# Load basic Image
FROM node:22-alpine

# Set work directory
WORKDIR /app

# Copy package jsons
COPY package*.json .

# Install dependencies
RUN npm ci

# Copy the source code
COPY src/index.js index.js

# Expose the application port
EXPOSE 3000

# Start Application
CMD ["npm","start"]


