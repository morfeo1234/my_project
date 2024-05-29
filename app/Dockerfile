# Usa l'immagine base di Python
FROM python:3.9-slim

# Imposta la directory di lavoro
WORKDIR /app

# Copia i file requirements.txt e installa le dipendenze
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

# Copia il contenuto della cartella app nel container
COPY . .

# Esponi la porta 5000
EXPOSE 5000

# Comando per eseguire l'app
CMD ["python", "app.py"]
