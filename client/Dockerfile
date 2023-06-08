# Use a base Node.js image with the desired version
FROM node:18

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the Next.js app files to the container
COPY . .

# Expose port 3000 (default Next.js development server port)
EXPOSE 3000

# Start the Next.js development server
CMD ["npm", "run", "dev"]