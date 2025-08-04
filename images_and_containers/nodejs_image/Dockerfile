FROM node:alpine



# Define working directory to the destiny dir
WORKDIR /app

# Copy package.json and package-lock.json to the image
COPY package*.json ./

# Install the deps
RUN npm install 


# Copy everything to the image
COPY . ./app

# Expose the port to our localhost
EXPOSE 80

# RUN The server
CMD [ "node","server.js" ]

