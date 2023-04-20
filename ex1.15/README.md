# Exercise 1.15

This image is a dockerized version of intentionally flawed project for Helsinki university's cyber security course.
So needless to say, that this project should never be used in any kind of production environment.

[Dockerhub link](https://hub.docker.com/r/faktatykki/cbs-project)

### Run the project

```
docker pull faktatykki/cbs-project
docker run -p 8000:8000 faktatykki/cbs-project
```

The application should be running in [localhost:8000](http://localhost:8000)
