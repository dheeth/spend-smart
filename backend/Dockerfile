FROM node:slim

# Set working directory for the build stage
WORKDIR /app

# Copy package.json for dependency installation
COPY package*.json ./

# Install dependencies in the builder stage

RUN npm install

COPY . .

# Define environment variables (replace with your actual variables)

ENV NODE_ENV=production

# Set working directory for the final image
WORKDIR /app

# Expose the port for the application
EXPOSE 3000

# Entrypoint to start the application
ENTRYPOINT ["npm", "start"]
