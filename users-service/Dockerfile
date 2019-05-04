# Use Node v4 as the base image.
# FROM node:4

# update node version
# 
# November 30, 2018 at 07:29 PM
# 4842f9314da0
# < 140 MB
# 
FROM node:10.15.3-jessie-slim

# Add everything in the current directory to our image, in the 'app' folder.
ADD . /app

# Install dependencies
RUN cd /app; \
    npm install --production

# Expose our server port.
EXPOSE 8123

# Run our app.
CMD ["node", "/app/index.js"]
