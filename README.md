# container-from-scratch-python
This is building a container from scratch

## Build the Container Yourself and Push to Docker Hub

```shell
# Build image *(If you want to develop yourself)* 
docker build --tag=app .

# List docker images
docker image ls

# Run my newly built container from source
docker run -it noahgift/cloudapp python app.py --name "Big John"

# Run my newly built container locally
docker run -t app python app.py --name "Big John"

# Push to Docker Hub
# Note:  You will need to change for your Docker Hub Repo
docker push noahgift/duke102:tagname

## Run it yourself

docker pull noahgift/cloudapp:latest
docker run -it noahgift/cloudapp bash 

#then run python app.py --help

# Pass in a command

docker run -it noahgift/cloudapp python app.py --name "Big John"
#the output
Hello Big John!

```

## Push to Amazon ECR

1.  Create ECR repository


### More things Do

* Lint the code with Github Actions (see the Makefile)
* Automatically build the container after lint, and push to DockerHub or some other Container Registery



