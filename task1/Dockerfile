# Based on the latest ubuntu
FROM ubuntu:latest

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software through APT using apt-get upgrade -y
RUN apt-get upgrade -y

# Install python3, python3-pip
RUN apt-get install -y python3 python3-pip

# Manage error when trying to install Python packages
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask with pip3
RUN pip3 install flask

# Working directory
WORKDIR /app

# Copy the Python file to Docker image
COPY api.py /app/api.py

# Expose port 5252
EXPOSE 5252

# Run Docker image
CMD ["python3", "api.py"]
