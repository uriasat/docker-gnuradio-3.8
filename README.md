# gnuradio-3.8

Docker build of gnuradio-3.8, from source, on Ubuntu 18.04.

Build locally using the build instructions, if you want.

Or, this image is also pushed to [Theseus Cores Docker Hub](https://hub.docker.com/r/theseuscores/gnuradio),
so you can jump straight to the "running" section without doing a local build.


## Build instructions

`docker build --tag theseuscores/gnuradio .`

There's also a number of override-able parameters in the Dockerfile that
can be used to specify Gnuradio and UHD configuration.

## Running

Run the docker image, with volume mounts for running gnuradio-companion
and a data directory:

```
./run-over-network
```

For an additional shell run:

```
docker exec -it gnuradio bash
```

To start and reattach to a stopped container:
```bash
docker start <container-name>
docker attach <container-name>
```
