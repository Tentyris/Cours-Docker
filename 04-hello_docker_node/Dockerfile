FROM node 

#Donne le répertoire de travail
WORKDIR /usr/src/app

#Copy le package Json dans le répertoir
COPY package.json /usr/src/app

#Copy Fait pareil avec le -lock
COPY package-lock.json /usr/src/app

#installe les dépendances
RUN npm install 

COPY . .

#Définie le port 3000 pour l'application
EXPOSE 3000

# lance l'aplication
CMD ["node", "app.js"]



