# Základný image
FROM python:3.11-slim

# Nastav pracovný priečinok
WORKDIR /app

# Skopíruj requirements a nainštaluj závislosti
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Skopíruj aplikáciu
COPY app.py .

# Nastav port
EXPOSE 8080

# Spusti aplikáciu
CMD ["python", "app.py"]

