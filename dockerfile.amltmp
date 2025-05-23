# Use an official Python 3.10.11 image
FROM python:3.10.11-slim

# Set the working directory
WORKDIR /app

# Copy the current directory contents to /app in the container
COPY . /app

# Upgrade pip and install dependencies
RUN pip install --no-cache-dir --upgrade pip && pip install --no-cache-dir -r requirements.txt

# Expose port 5000 (assuming Flask default port)
EXPOSE 5000

# Run serve_model.py on container start
CMD ["python", "serve_model.py"]