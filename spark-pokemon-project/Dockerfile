# Use the Jupyter PySpark Notebook as the base image
FROM jupyter/pyspark-notebook

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Make port 8888 available to the world outside this container
EXPOSE 8888

# Run Jupyter Notebook on container start, accessible to any IP
CMD ["start-notebook.sh", "--NotebookApp.allow_origin='*'", "--NotebookApp.ip='0.0.0.0'", "--NotebookApp.open_browser=False"]
