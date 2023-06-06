# set the base image
FROM python:3.9-slim-buster

# set the working directory in the container
WORKDIR /app

# copy the requirements file to the container
COPY requirements.txt .

# install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# copy the rest of the application files to the container
COPY . .

# expose the port
EXPOSE 5000

# set the command to start the application
CMD ["python", "app.py"]
