# checking image running 
docker image ls

# pulling docker image
docker image pull image

# to be root user
newgrp docker 

# check running container
docker container ls
#all 
docker container ls -a

#start container
docker container start {name}

#stop container
docker container stop {name}

# remover container
docker container rm {container}

# run container interactive terminal
docker container run -ti {image}
# with port and bash (80 HTTP port (VM) -- 5000 Container)
docker container run -ti  --{name} -p 80:5000 python bash

# creating image
docker build <dockerfile location> --help

# attch ourseleve to container
docker container attach
# exit container 
ctrl p + ctrl q

#creating image from container -> get hash
docker commit {name} 
docker commit bank bankapp:1.0

# retag
docker tag bankapp:1.0 {repo name/banking:1.0
docker tag originalname newname

#pushing to docker
docker push kingmant/banking:1.0

# sharing immage
-create the image
-docker username and TD

docker login (or use a argument)
docker push

python -m gunicorn -w 4 application:app -b 0.0.0.0
EntryPoint cant be overwrite. CMD can be over written

# building the image as tag and the path (.)
docker build
docker build -t urlimage .

dockerfile: 

#rename image 
docker tag



















