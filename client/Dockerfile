FROM node:alpine

# Adding env variables to solve 2 bugs, issues 8688 and 11779, can be found on react github repo
ENV CI=true
ENV WDS_SOCKER_PORT=0

WORKDIR /app
COPY package.json ./
RUN npm install
COPY ./ ./

CMD ["npm","start"]