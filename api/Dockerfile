# Utiliser l'image de base alpine pour construire l'image Docker
FROM node:alpine

# Définir le répertoire de travail à l'intérieur du conteneur
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package*.json ./

# Exécuter la commande npm install à l'intérieur du conteneur Docker
RUN npm install

# Copier tous les fichiers et répertoires restants depuis le répertoire local vers le répertoire /app dans le conteneur Docker
COPY . .

# Définir la commande par défaut à exécuter lorsque le conteneur Docker est démarré
CMD ["npm", "start"]
