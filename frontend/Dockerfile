# image de base
FROM node:8.11-alpine

# dossier d'éxecution
WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

# install application dependence
COPY package*.json ./

# installation dependances 
RUN npm install

# copy app files
COPY . .

# port d'écoute
EXPOSE 3000

# commande à lancer
CMD ["npm" , "start"]