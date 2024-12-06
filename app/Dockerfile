# Usar una imagen base oficial de Node.js
FROM node:18-alpine

# Definir el directorio de trabajo dentro del contenedor
WORKDIR /usr/src/app

# Copiar los archivos package.json y package-lock.json (si existe) para instalar las dependencias
COPY package*.json ./

# Instalar las dependencias de la aplicación
RUN npm install

# Copiar el resto de los archivos del proyecto al contenedor
COPY . .

# Exponer el puerto 3000
EXPOSE 3000

# Definir el comando para ejecutar la aplicación cuando el contenedor se inicie
CMD ["node", "app.js"]
