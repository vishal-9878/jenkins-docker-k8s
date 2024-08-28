# jenkins-docker-k8s
## commands to build and run docker
docker image build -t custom-jenkins-docker .
docker run -it -p 8080:8080 -p 50000:50000 -v /var/run/docker.sock:/var/run/docker.sock -v jenkins_home:/var/jenkins_home custom-jenkins-docker