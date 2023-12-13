# Utilizar la imagen base de Node.js 14
FROM node:14

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar el código del servidor al directorio de trabajo
COPY . ./server

# Instalar las dependencias del servidor
RUN npm install

# Definir una variable de entorno para la clave de conexión a MongoDB
ENV DB_URL_ATLAS="mongodb+srv://ocanhapcs:mWW5qFhMpagiI1Xi@cluster0.ljhdqgm.mongodb.net/"

# Iniciar el servidor
CMD ["sh", "-c", "cd server && npm start"]
