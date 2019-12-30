# production
FROM node:12.4.0-alpine
ENV NODE_ENV production

# deps
WORKDIR /opt/app
COPY package.json .
COPY yarn.lock .
RUN yarn --prod

# source code
COPY index.js index.js

EXPOSE 8080

CMD ["node", "index.js"]
