# image dockerfile a crée 
FROM python:3.11-slim

# set the working directory in the container
WORKDIR /app

# copy the requirements file into the container
COPY requirements.txt .

# install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# copy the rest of the application code into the container
COPY . .

# expose the port that the application will run on
EXPOSE 5001
# command to run the application
ENTRYPOINT ["python", "app_satisfaction.py"]