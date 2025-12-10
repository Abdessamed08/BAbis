# Utilise Python
FROM python:3.11-slim

# Dossier de travail
WORKDIR /app

# Copier tout le contenu
COPY . .

# Installer les dépendances si tu as un requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Commande pour lancer ton app
CMD ["python", "app.py"]

