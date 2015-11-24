# Devops-HW4 - Advanced Docker

This repository has instructions on how to perform File IO, use Ambassador pattern and deploy blue/green deployment using Docker containers. 

<h3>File IO</h3>
In order to demonstrate communication between two linked containers in docker we use socat and linking. 
To see the working of this functionality follow the below steps:
* Clone this repository into your local file system.
* CD into the FileIO directory. 
* There are two folders one each for container1 and container2. 
* CD into the container1 folder and execute the following command to build the image for the container:</br>

  ```docker build -t container1image ```</br>
  
* Now run ``` docker images ``` to check whether the image has been built.
* Next run</br>

  ``` docker run -d --name container1 container1image ``` </br>
 
  in order to start the container. 
* Run ``` docker ps ``` in order to check whether this container is running. 
* In this container socat is currently running which exposes the port 9001 and shows the content of file.txt on this port.
* Now CD to container2 and run the following command </br>

  ``` docker build -t container2image ```</br>
  
*
