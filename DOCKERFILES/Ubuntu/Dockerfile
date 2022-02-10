FROM ubuntu:20.04

#Mise à jour et ajout de paquet
RUN apt update
RUN apt upgrade -y
RUN apt install vim -y
RUN apt install sudo -y
RUN apt install nginx -y
#Port utilisé
EXPOSE 80

VOLUME var/www/html

#Démarrage du service nginx
CMD ["/sbin/nginx"]