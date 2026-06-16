# 1. Usa una versión oficial y ligera de Node.js
FROM node:18-alpine

# 2. Define la carpeta de trabajo dentro del contenedor
WORKDIR /app

# 3. Copia los archivos de dependencias primero (optimiza el caché)
COPY package*.json ./

# 4. Instala las dependencias
RUN npm install

# 5. Copia el resto de tu código
COPY . .

# 6. Expone el puerto que usará tu API de Express (ej. 5000)
EXPOSE 5000

# 7. Comando para iniciar tu servidor en modo desarrollo
CMD ["npm", "run", "dev"]