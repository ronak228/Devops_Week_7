# Use the official Node.js image as the base image
FROM node:18

# Create and set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files to the container
COPY . .

# Expose the port your app will run on
EXPOSE 5555

# Start the app
CMD ["node", "index.js"]
