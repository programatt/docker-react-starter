FROM node:8.1

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# add `/usr/src/node_modules/.bin` to $PATH
ENV PATH /usr/src/app/node_modules/.bin:$PATH

# install and cache app dependencies
ADD package.json /usr/src/app/package.json
RUN npm install

EXPOSE 8080

CMD ["npm","start"]