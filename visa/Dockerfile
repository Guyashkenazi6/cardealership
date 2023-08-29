# Use the official Python 3.10 base image
FROM python:3.10

# Set the working directory inside the container
WORKDIR /app

RUN pip install fastapi uvicorn pymongo 

# Copy your Python script into the container
COPY visa.py /app

# Install any dependencies your script might have
# For example, if you're using pymongo, you can install it like this:
# RUN pip install pymongo

EXPOSE 9010

# Run the Python script
CMD ["python", "visa.py"]
