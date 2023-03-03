# Establece la imagen base
FROM ubuntu:latest

# Actualiza el sistema y establece las variables de entorno
RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

# Define el directorio de trabajo
WORKDIR /app

# Copia los archivos necesarios al contenedor
COPY app.py .

# Establece el comando predeterminado que se ejecutará cuando se inicie el contenedor
CMD [ "python3", "app.py" ]


#Con cada cambio en el archivo python debo builder y run
#docker build -t dockerfile-py .
#docker run --rm -it --name my-pythoh-container dockerfile-py