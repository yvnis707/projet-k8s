FROM python:3.11-slim

WORKDIR /app

RUN pip install flask

COPY app.py .

# Bonne pratique sécurité : ne pas lancer en root
RUN useradd -m appuser
USER appuser

EXPOSE 5000

CMD ["python", "app.py"]
