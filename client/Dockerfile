# Use an official Node.js runtime as a parent image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy the package.json and package-lock.json files into the container
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of your Next.js app into the container
COPY . .

# Expose port 3000 for the Next.js app
EXPOSE 3000

# Run the development server with hot reload
CMD ["npm", "run", "dev"]