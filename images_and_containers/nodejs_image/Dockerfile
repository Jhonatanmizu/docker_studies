FROM node:alpine


# Copy everything to the image
## The first dot means copy all in the current dir and the next dot is the destiny dir
COPY . ./app

# Define working directory to the destiny dir
WORKDIR /app

# Install the deps
RUN npm install 

# Expose the port to our localhost
EXPOSE 80

# RUN The server
CMD [ "node","server.js" ]

