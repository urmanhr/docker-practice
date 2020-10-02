# from image
FROM node:alpine
# include dependency
COPY ./package.json ./
RUN npm install
COPY ./ ./
#run command
# EXPOSE 8080
CMD [ "npm","start" ]