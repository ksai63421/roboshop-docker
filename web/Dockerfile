FROM nginx
# I am  removing default index.html configuration 
RUN rm -rf /usr/share/nginx/html/index.html 
# I am copying our default reverse proxy conguration
COPY roboshop.conf /etc/nginx/default.d/roboshop.conf 
# I am copying our code 
ADD static /usr/share/nginx/html/