# Usando una imagen de Node.js como base
FROM node:18-alpine

# Estableciendo el directorio de trabajo en la aplicación backend
WORKDIR /app/backend
RUN chmod 755 /app

# Copiando el archivo package.json e instalando las dependencias
COPY package.json .
#COPY package-lock.json .
RUN npm install

# Copiando el código fuente del backend al contenedor
COPY . .

# Exponiendo el puerto 8080
EXPOSE 8080

# Comando para iniciar la aplicación backend
CMD npm start
