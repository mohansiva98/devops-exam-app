FROM python:3.8-slim

WORKDIR /app

<<<<<<< HEAD
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .  # This should copy templates/ if it exists

# Optional: ensure templates is copied explicitly (extra-safe)
COPY templates/ templates/

CMD ["python3", "app.py"]

=======
# Install dependencies
COPY requirements.txt .
RUN pip install -r requirements.txt

# Install Gunicorn
RUN pip install gunicorn

# Copy the application code
COPY . .

# Expose the port
EXPOSE 5000

# Run the app using Gunicorn (replace 'app' with the name of your Flask app)
CMD ["gunicorn", "--bind", "0.0.0.0:5000", "app:app"]
>>>>>>> 9ebad62a012591ba8b596595539db0f442e55307
