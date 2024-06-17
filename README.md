# Syyclops
# Ifc-based BIM application

## Overview:
This project uses the IfcOpenShell library to process Building Information Model (BIM) files in the IFC format. The application reads an IFC file, extracts relevant data about building elements, their properties, relationships and performs simple analysis (total wall area and number of elements), and saves the processed data to two separate JSON files. This project is containerized using Docker to ensure a consistent runtime environment.

## Instructions to clone the repo and run the app

1.	Clone the Repository:
•	Clone this repository to your local machine.

```sh
git clone https://github.com/NishchithAnanthaRamu/Ifc-BIM-processing-app---Syyclops.git
```

2.	Updating the IFC file path in the script:

•	Update the script to use the correct path to your IFC file.

3.	Build the Docker Image:

•	Build the Docker image using the provided Dockerfile.

```sh
docker build -t ifcopenshell-app .
```
4.	Run the Docker Container:

```sh

docker run -d -v container_volume:/app image_ID
```
This command maps the current directory's docker volume ‘container_volume’ to the container's /app directory and hence sets the JSON's output directory.



