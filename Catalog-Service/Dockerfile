# Use an official Python runtime as a parent image 
FROM python:2.7-slim
# Set the working directory to /app
WORKDIR /app1
# Copy the current directory contents into the container at /app
ADD . /app1
# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt
# Make port 90 available to the world outside this container
EXPOSE 80
# Define environment variable
ENV NAME World
# Run app.py when the container launches
CMD ["python", "app1.py"]
