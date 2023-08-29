# Use the official Python 3.10 base image
FROM python:3.10

# Set the working directory inside the container
WORKDIR /app

RUN pip install fastapi uvicorn requests pymongo

# Copy your Python script into the container
COPY main.py /app

# Install any dependencies your script might have
# For example, if you're using pymongo, you can install it like this:
# RUN pip install pymongo

EXPOSE 9000

# Run the Python script
CMD ["python", "main.py"]
