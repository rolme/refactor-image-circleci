# Refactor Server Image for CircleCI

This is a docker image used by circleCI to test the Refactor Service. It is based on node:12.12.0-buster image that also installs AWS CLI and Python.


## Install Docker
[Download and sign up here](https://hub.docker.com/?overlay=onboarding)
Ask Admin to invite you to Refactor Docker

## Testing and deployment

```sh
docker build -t rolme/refactor-image-circleci .
docker run -it --rm rolme/refactor-image-circleci
docker login && docker push rolme/refactor-image-circleci
```

## References

[How to create a docker image](https://www.scalyr.com/blog/create-docker-image/)
