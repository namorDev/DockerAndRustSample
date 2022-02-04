# DockerAndRustSample
Simple Rust demo application which runs in a docker container

# Prerequisites
- Docker installed
- Only tested on Linux

# Build
1. build and run locally without docker: 
    1. `mkdir build`
    2. `cd build`
    3. `rustc ../HelloDocker.rs`
    4. `./HelloDocker`

    You can also build it with cargo. See: https://doc.rust-lang.org/cargo/getting-started/first-steps.html

2. Build with Docker
    1. Dockerfile must be in the same directory as rust application binary
    2. Build Docker image with `docker build -t my-docker-image-name .` (You need to be inside build directory)
    3. Check if docker image is generated with `docker images`
    4. Run image with `run my-docker-image-name`

# Resources
- https://blog.knoldus.com/containerize-rust-application-with-docker/