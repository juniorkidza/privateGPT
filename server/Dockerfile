# Use a base Python image
FROM python:3.8

# Set the working directory in the container
WORKDIR /app

# Copy the requirements.txt file to the container
COPY requirements.txt .

# Install the Python dependencies
RUN pip install -r requirements.txt

# Copy the privateGPT.py file to the container
COPY privateGPT.py .

# Expose port 5000
EXPOSE 5000

# Run the privateGPT.py script
CMD ["python", "privateGPT.py"]