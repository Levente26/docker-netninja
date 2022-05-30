# pull node image
FROM node:16-alpine

RUN npm install -g nodemon

# working directory
WORKDIR /app

COPY package.json . 

# install dependencies to the image
RUN npm install 

# copy the source files to the image
COPY . .

# port number
EXPOSE 4000

CMD ["npm", "run", "dev"]


# all of them are LAYERS