# ini Hello World

This is an example of how to run a simple HTML/CSS/JS site on ini. 

## Deployment

### Build and host the Docker image

The first thing you'll need to deploy on ini is a docker image. This step will build a docker image from the Dockerfile and push it to Docker Hub. 

You can skip this if you already have a docker image you want to run on ini. You can also fork this repo and setup Docker Hub to automatically build from GitHub.

Note ini needs a public repository for now. Also note that you should specify an explicit version rather than `latest` so you can update the image as required. 

```
# Change below to your user/repo

docker build . -t inichain/inichain-hello-world:release-v0.1.0
docker push inichain/inichain-hello-world:release-v0.1.0
```

You can now update deploy.yml to use your user/repo.
