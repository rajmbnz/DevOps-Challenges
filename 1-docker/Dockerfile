FROM node:12-alpine
RUN useradd -u 1001 bmadaiah
USER bmadaiah
WORKDIR /app
COPY package.json yarn.lock ./
RUN yarn install --production
COPY . .
CMD ["node", "src/index.js"]
