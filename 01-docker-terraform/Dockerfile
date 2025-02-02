FROM python:3.12.8-alpine3.21

RUN apk add --no-cache bash

# Set the working directory
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Install jupyter
RUN pip install --no-cache-dir jupyter

# Run Jupyter server
CMD ["tail", "-f", "/dev/null"]
