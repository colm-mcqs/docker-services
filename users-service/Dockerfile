# use Node v6 as the base image
FROM node:6

# Run Node
CMD ["node"]

# Add everything in the current directory to our image in the 'app' folder
ADD . /app

# install dependencies

RUN cd /app; \
    npm install --production

# expose server port
EXPOSE 8123

#Run the App
CMD ["node", "/app/index.js"]