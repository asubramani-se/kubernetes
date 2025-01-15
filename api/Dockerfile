# Use the official Python image
FROM python:3.9-slim

# Set the working directory
WORKDIR /app

# Copy your application code into the container
COPY . /app

# Install dependencies from requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port your app runs on
EXPOSE 5000

# Run the application
CMD ["python", "app.py"]