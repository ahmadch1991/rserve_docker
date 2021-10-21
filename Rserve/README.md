***Enviournment must be re-build and deployed on docker after every major addition in R scripts.***


**To build a new R infrastructure, open CLI inside the downloaded directory and run the command:**

docker build -t rserve Rserve/ --no-cache

**Once the image is built, deploy the image on the docker container using the command:**

docker run --name EnvR -p 6311:6311 --rm rserve:latest

** Once the docker is deployed, then type the following command to get the IP and other network details of the image:**

docker network inspect bridge

**Get IP of image EnvR and use it in DIME Configuraitons**

