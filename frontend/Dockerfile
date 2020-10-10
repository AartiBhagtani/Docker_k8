# block for build container
FROM node:alpine
WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
RUN npm run build


# block for run builder
FROM nginx
COPY --from=0 /app/build /usr/share/nginx/html
    