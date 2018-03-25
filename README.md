# docker-scala-native
This repository offers alpine-based build and runtime environment for [scala-native][].

[scala-native]:https://github.com/scala-native/scala-native


# Usage
## For build (and runtime)
![](https://img.shields.io/docker/automated/amaya382/scala-native-builder.svg)
![](https://img.shields.io/docker/build/amaya382/scala-native-builder.svg)
![](https://img.shields.io/microbadger/layers/amaya382/scala-native-builder/latest.svg)
![](https://img.shields.io/microbadger/image-size/amaya382/scala-native-builder/latest.svg)

Use `amaya382/scala-native-builder`

## For runtime only
![](https://img.shields.io/docker/automated/amaya382/scala-native.svg)
![](https://img.shields.io/docker/build/amaya382/scala-native.svg)
![](https://img.shields.io/microbadger/layers/amaya382/scala-native/latest.svg)
![](https://img.shields.io/microbadger/image-size/amaya382/scala-native/latest.svg)

Use `amaya382/scala-native`


# Example
```sh
docker run -it amaya382/scala-native-builder sh
```

In the container,
```sh
sbt new scala-native/scala-native.g8 # name=scala-native-seed-project
cd scala-native-seed-project
sbt run # "Hello, World!"
```

And you should find an executable file in `target/scala-2.11`.


# Acknowledgement
* [rwhaling/dinosaur](https://github.com/rwhaling/dinosaur)

