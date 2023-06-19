FROM node:10.16-alpine
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install --silent
RUN npx browserslist@latest --update-db
COPY . .
EXPOSE 3000
CMD ["npm","start"]