# Descargar la imagen de ubuntu
FROM ubuntu:22.04
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# Actualizar la lista de actualizaciones y corregir problemas de descarga
RUN apt-get update --fix-missing

# Actualizar la imagen
RUN apt-get upgrade -y --fix-missing

# Instalar Python 3
RUN apt-get install python3 -y --fix-missing

# Copiar la carpeta webapp
COPY ./webapp /home/webapp

# Establecer directorio de trabajo
WORKDIR /home/webapp

# Instalar pip y corregir problemas de descarga
RUN apt-get install python3-pip -y --fix-missing

# Instalar las librerías desde el archivo requirements.txt
RUN pip3 install -r requirements.txt

# Abrir el puerto 8080
EXPOSE 8080

# Ejecutar la aplicación
CMD [ "python3", "app.py" ]
