FROM 172.18.63.26:5000/node:14-alpine

RUN apk update && apk add bash

COPY ./node_modules /code/node_modules

# To make sure symlink paths are not broken
COPY ./.next /code/.next

COPY ./package.json /code


CMD ["node_modules/.bin/next", "start"]

WORKDIR /code
