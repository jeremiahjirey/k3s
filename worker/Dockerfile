FROM node:latest
WORKDIR /app
RUN apt-get update  && apt-get install -y git
RUN git clone https://github.com/handipradana/nodejsbasic.git .
RUN npm install --prefix
RUN npm install -g pm2
EXPOSE 8000
CMD ["pm2-runtime", "npm", "--", "run", "start-prod"]

