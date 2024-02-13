FROM nginx
# I am  removing default index.html configuration 
RUN rm -rf /usr/share/nginx/html/index.html
RUN rm -rf /etc/nginx/nginx.conf
RUN rm -rf /etc/nginx/conf.d/default.conf  
# I am copying our default reverse proxy conguration
COPY roboshop.conf /etc/nginx/default.d/roboshop.conf 
ADD static /usr/share/nginx/html/ 
