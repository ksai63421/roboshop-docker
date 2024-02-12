FROM node:14
EXPOSE 8080
# just creating one dedicated directory for application
WORKDIR /opt/server
COPY package.json .
COPY server.js .
# install the dependencies
RUN npm install 
ENV MONGO=true 
useUnifiedTopology: true
CMD ["node", "server.js"]