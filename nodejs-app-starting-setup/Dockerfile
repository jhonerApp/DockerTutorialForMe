FROM node 
# node - image that existing in docker hub
# cached locally

WORKDIR /app

# setting working directory inside the docker container
# this tells docker that all the subsequent commands will be executed from this folder
# RUN npm install runs all the files inside your workdir


COPY . /app

# Format COPY (.)1st path (.)2 path or create subfolder ex: ./app or / (means current workdir or relative path)

# .. specifiy 2 paths, 
# >  1st path or dot is outside of container,outside of the image
# where the files leave that should be copied into the image or local folder
# where the files located in your pc(excluding the Dockerfile).

# 2 path  or dot is the the path inside of image where those files should be stored.


RUN npm install

EXPOSE 80 
# Expose port is optional


CMD ["node","server.js"]

# RUN APPLICATION