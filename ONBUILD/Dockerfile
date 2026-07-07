FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/*
# This instruction runs when someone use this image
ONBUILD COPY src/ /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]