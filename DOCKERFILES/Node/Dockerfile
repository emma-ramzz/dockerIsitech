FROM node:10-alpine

#Permet de définir le dossier de travail pour les autre sinstrctions du dockerfile (RUN, CMD, ENTRYPOINT, ADD)
WORKDIR /usr/src/app 
COPY package*.json ./

RUN npm install

COPY . .
EXPOSE 3000

CMD [ "npm","start" ]