# Use an official Python runtime as a parent image
FROM python

# Set the working directory in the container
WORKDIR /poll

# Copy the current directory contents into the container at /usr/src/app
COPY . .

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Run app.py when the container launches
CMD ["flask", "run", "--host=0.0.0.0", "--port=80"]
