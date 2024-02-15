FROM node:14.21.3-alpine3.17 
EXPOSE 8080
# just creating one dedicated directory for application
# we are creating one group cart and creating one user cart and then adding the cart user to cart group
RUN addgroup -s cart && adduser -s cart cart 
WORKDIR /opt/server
RUN chown -R cart:cart /opt/server
USER cart 
COPY package.json .
COPY server.js .
# install the dependencies
RUN npm install 
CMD ["node", "server.js"]
# we use system user they are not humans and they are represent the application
