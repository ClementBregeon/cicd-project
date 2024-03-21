# Utiliser une image Python officielle légère
FROM python:3.9-slim

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier les fichiers de dépendances
COPY requirements.txt ./

# Installer les dépendances
RUN pip install --no-cache-dir -r requirements.txt

# Copier le fichier app.py dans le conteneur
COPY app.py .

# Exposer le port sur lequel l'application Flask écoute
EXPOSE 5000

# Commande pour démarrer l'application Flask
CMD ["python", "app.py"]
