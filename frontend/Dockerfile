FROM nginx:1.22
COPY ./* /usr/share/nginx/html/
RUN chgrp -R root /var/cache/nginx /var run /var/log/nginx && \
    chmod -R 770 /var/cache/nginx /var/run /var/log/nginx
EXPOSE 81
CMD [ "nginx", "-g", "daemon off;" ]
