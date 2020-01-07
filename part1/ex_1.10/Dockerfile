FROM node:10
ADD frontend-example-docker /app
WORKDIR /app
RUN npm install
RUN npm run build
EXPOSE 5000
CMD ["npm","start"]


