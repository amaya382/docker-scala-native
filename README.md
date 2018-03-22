# docker-scala-native
This repository offers alpine-based build and runtime environment for [scala-native][].

[scala-native]:https://github.com/scala-native/scala-native


# Usage
## For build (and runtime)
Use `amaya382/scala-native-builder`

## For runtime only
Use `amaya382/scala-native`


# Example
```sh
docker run -it amaya382/scala-native-builder sh
```

In container,
```sh
sbt new scala-native/scala-native.g8 example-project
cd example-project
sbt run # "Hello World"
```

And you should find an executable file in `target/scala-2.11`.

