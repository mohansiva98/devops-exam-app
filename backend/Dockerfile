# Dockerfile
FROM python:3.8-slim

# Set working directory
WORKDIR /app

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
