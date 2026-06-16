# 1. Versión de Node
FROM node:18-alpine

# 2. Carpeta de trabajo
WORKDIR /app

# 3. Copiar dependencias
COPY package*.json ./

# 4. Instalar dependencias
RUN npm install

# 5. Copiar el código fuente
COPY . .

# 6. Vite suele usar el puerto 5173
EXPOSE 5173

# 7. Inicia Vite exponiendo la red para que sea accesible fuera del contenedor
CMD ["npm", "run", "dev", "--", "--host"]