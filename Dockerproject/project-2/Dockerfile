from node:18.19.0-alpine3.18
WORKDIR /app
COPY package.json ./
RUN npm install
COPY . ./
RUN npm run build
CMD ["npm", "run", "start"]
