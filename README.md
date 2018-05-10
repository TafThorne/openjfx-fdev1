# clang-fdev1
Dockerfile that sets up a basic gcc & OpenJFX toolkit Debian environment with a
number of libraries configured

The Docker Image is listed on Docker Hub:
https://hub.docker.com/r/tafthorne/openjfx-fdev1/

To pull the image:

 docker pull tafthorne/openjfx-fdev1

An overview of the included libraries is given below.

## Using This Image
The expected way to use this image is to navigate to the working directory
where your source code resides and start an interactive session.

  docker run -ti --volume="${PWD}:/shared" -w "/shared" tafthorne/openjfx-fdev1

Then within the running container you can call make or gcc as if it were
a native tool.  The libraries added to this image will be in the global include
path.

## OpenJFX

OpenJFX is the open source home of JavaFX development. The goal of OpenJFX is
to build the next-generation Java client toolkit.
* http://openjdk.java.net/projects/openjfx/

## Contributing

Please see the notes in CONTRIBUTING.md.

