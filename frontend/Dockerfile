# Usando una imagen de Node.js como base
FROM node:18-alpine

# Estableciendo el directorio de trabajo en la aplicación frontend
WORKDIR /app/frontend
RUN chmod 755 /app

# Copiando el archivo package.json e instalando las dependencias
COPY package.json .
#COPY package-lock.json .
RUN npm install

# Copiando el código fuente del frontend al contenedor
COPY . .

# Exponiendo el puerto 3000
EXPOSE 3000

# Comando para iniciar la aplicación frontend
CMD npm run dev
