FROM ubuntu:latest

# Install Docker
RUN apt-get update && \
    apt-get install -y docker-ce && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any other dependencies
RUN apt-get update && \
    apt-get install -y your_dependency_package && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Specify the command to run on container start
CMD ["/bin/bash"]

