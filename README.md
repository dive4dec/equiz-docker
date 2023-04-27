# equiz-docker

A customized E-quiz dockerfile based on Bitnami Moodle
- integrated with popular question types and related question behaviours, e.g CodeRunner, STACK 
- integrated with some useful plugins, e.g Collapsed Topics
- configure php-fpm to accelerate php requests handling
- fix some LTI issues

## Building and pushing the custom images

Push the images to localhost or dockerhub<br />

Example of building the moodle image and push to localhost:
```
docker build --no-cache -t localhost:32000/bitnami_moodle_custom:test1 .
docker push localhost:32000/bitnami_moodle_custom:test1
```

Example of building the moodle image and push to dockerhub:
```
docker build --no-cache -t <dockerhub account>/<dockerhub repo>:<tag> .
docker push <dockerhub account>/<dockerhub repo>:<tag>