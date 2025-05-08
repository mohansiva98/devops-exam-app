FROM python:3.10-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .  # This should copy templates/ if it exists

# Optional: ensure templates is copied explicitly (extra-safe)
COPY templates/ templates/

CMD ["python3", "app.py"]

