# Use an official Python runtime as a parent image
FROM python:2.7-slim

#Setting proxy.
ENV http_proxy http://172.16.19.10:80/
ENV https_proxy https://172.16.19.10:80/


# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Make port 80 available to the world outside this container
EXPOSE 80

# Define environment variable
ENV NAME World

# Run app.py when the container launches
CMD ["python", "app.py"]
