# Hello Docker in Cloud Foundry!

This is a very simple demo of a python flask application in a docker container which can be deployed to cloud foundry. Below are general steps to deploy.

1) build your image

    docker build -t your.repo.com/your_namespace/friendlyhello:latest

2) push your image

    docker push your.repo.com/your_namespace/friendlyhello:latest

3) Adjust manifest.yml to suite your needs, especially the image location and namespace.
4) push your app

    cf push

And now, assuming docker images are enabled in your Cloud Foundry foundation, you should see friendlyhello in your list of apps.
