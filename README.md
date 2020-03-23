# Refactor Server Image for CircleCI

This is a docker image used by circleCI to test the Refactor Service. It is based on node:12.12.0-buster image that also installs AWS CLI and Python.

## Testing and deployment

```sh
docker build -t rolme/refactor-image-circleci .
docker run -it --rm rolme/refactor-image-circleci
docker login && docker push rolme/refactor-image-circleci
```

## References

[How to create a docker image](https://www.scalyr.com/blog/create-docker-image/)