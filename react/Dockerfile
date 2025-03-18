FROM node:22.13.0
ENV NODE_ENV=development

WORKDIR /usr/src/app

COPY package.json ./
COPY package-lock.json ./
RUN npm install

COPY . .

CMD ["npm", "start"]
