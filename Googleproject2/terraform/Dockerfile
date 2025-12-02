# Use official Python runtime as base image
FROM python:3.9-slim

WORKDIR /app

# Copy requirements and install
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy application files
COPY app.py .               
COPY templates_clean/ ./templates  

# Expose port
EXPOSE 5000

# Run app
CMD ["python", "app.py"]
