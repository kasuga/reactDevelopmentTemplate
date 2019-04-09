FROM node:latest

EXPOSE 8080
WORKDIR /app

RUN npm init -y
RUN npm install --save react react-dom
RUN npm install --save-dev webpack webpack-cli webpack-dev-server babel-loader @babel/core babel-preset-react @babel/preset-env html-webpack-plugin

COPY ./webpack.config.js /app/webpack.config.js



CMD /app/node_modules/.bin/webpack-dev-server --hot
