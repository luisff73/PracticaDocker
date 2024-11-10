FROM node:16-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm install -g serve
RUN npm run build

EXPOSE 8080
CMD ["serve", "-s", "dist", "-l", "8080"]