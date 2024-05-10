# Use the official Python image as base
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy the Python script into the container
COPY httpServer.py .

# Install dependencies if needed (not necessary for this simple script)

# Expose port 8000
EXPOSE 8000

# Run the Python script when the container launches
CMD ["python", "httpServer.py"]
