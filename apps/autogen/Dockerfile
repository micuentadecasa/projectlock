# Use a Python base image
FROM python:3.8

# Set the working directory in the container
WORKDIR /app

# Copy the Python requirements file and install dependencies
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of your app's source code from your host to your app's working directory in the container
COPY . .

# Expose the port your app runs on
EXPOSE 5000

# Run the application
CMD ["python", "run.py"]