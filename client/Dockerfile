# Utilizar la imagen base de Node.js 14
FROM node:14

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar el código del cliente al directorio de trabajo
COPY . ./client

# Instalar las dependencias del cliente
RUN npm install

# Exponer el puerto utilizado por el cliente
EXPOSE 5173

# Iniciar el cliente
CMD ["sh", "-c", "cd client && npm run dev"]