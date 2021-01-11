# vue-docker-example

A test project that dockerizes a [Vue](https://vuejs.org/) project
having [VueRouter](https://router.vuejs.org/) with history mode.

## How to run

Build docker image:

```
docker build -t vue-docker-example .
```

Create and run docker container:

```
docker run -it -p 8080:80 --rm --name vue-docker-example-1 vue-docker-example
```

After that go to http://localhost:8080/ to view the result.
