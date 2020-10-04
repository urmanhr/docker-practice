FROM node:alpine
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

FROM nginx as run
COPY --from=0 /app/build /usr/share/nginx/html