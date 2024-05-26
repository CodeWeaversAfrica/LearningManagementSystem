# frontend/Dockerfile

# Use official Node image as a parent image
FROM node:16.13.1

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend code
COPY . .

# Expose port 5173 for the development server
EXPOSE 5173

# Start Vite development server
CMD ["npm", "run", "dev", "--", "--host"]
