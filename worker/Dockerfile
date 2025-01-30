FROM node:latest
RUN apt-get update && apt-get install -y git
WORKDIR /app
RUN git clone https://github.com/dihkaw/showipserverwithnodejs.git .
RUN npm install
RUN npm install -g pm2
EXPOSE 5000
CMD [ "pm2runtime", "index.js" ]