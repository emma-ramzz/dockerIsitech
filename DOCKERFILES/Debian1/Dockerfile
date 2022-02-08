FROM debian:latest
RUN apt-get update -yq \
&& apt-get install curl gnupg -yq \
&& curl -sL https://deb.nodesource.com/setup_10.x | bash \
&& apt-get install nodejs -yq \
&& apt-get clean -y

ADD . /app/
WORKDIR /app
RUN npm install 
#Port sur lequel l'app écoute
EXPOSE 2368
#Repo partagé avec l'hote
VOLUME /app/logs

CMD npm run start