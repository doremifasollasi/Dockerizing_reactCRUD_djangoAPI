# Use an official node runtime as a parent image
FROM node:14

WORKDIR /app/


# 
# Install dependencies
COPY package.json yarn.lock /app/
# 
RUN npm install
#

RUN npm install --save bootstrap
RUN npm install --save react-router-dom
RUN npm install react-scripts --save
# 

# Add rest of the client code
COPY . /app/

EXPOSE 3000


# 
CMD npm start
# 


