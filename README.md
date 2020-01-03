# nlpreviz-docker
Dockerfile for [NLPReViz](https://github.com/NLPReViz/) on OpenJDK7
If you don't have [Docker](https://www.docker.com/), download and install from this link: https://docs.docker.com/get-docker/

## Running NLPReViz using Docker:

### Clone repository
```
git clone https://github.com/NLPReViz/nlpreviz-docker
cd nlpreviz docker
```

### Build image from Dockerfile
`docker build -t nlpreviz .`

### Run the image
`docker run -dit -p 8080:8080 --name emr_vis_web nlpreviz`

Point your browser to <localhost|DOCKER_IP>:8080/emr-vis-web/app. Enter `username` and `password` as defaults to login. Use `docker-machine ip` to confirm your local docker IP. For customization deployments, refer to documentation available on the main [NLPReViz](https://github.com/NLPReViz/) projects.
