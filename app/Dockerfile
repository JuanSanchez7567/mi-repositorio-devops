FROM python:3.9

WORKDIR /app

# Copiar el archivo de requisitos primero para aprovechar el cache de Docker
COPY requirements.txt .

# Instalar las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Copiar el resto de los archivos
COPY . .

# Exponer el puerto que usará tu aplicación
EXPOSE 5000

# Comando para iniciar la aplicación
CMD ["python", "app.py"]

