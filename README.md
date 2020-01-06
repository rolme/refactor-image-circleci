```sh
docker build -t rolme/refactor-image-circleci .
docker run -it --rm rolme/refactor-image-circleci
docker login && docker push rolme/refactor-image-circleci
```