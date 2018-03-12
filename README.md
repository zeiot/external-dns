# RPI Ark

* Master: [![pipeline status](https://gitlab.com/zeiot/rpi-ark/badges/master/pipeline.svg)](https://gitlab.com/zeiot/rpi-ark/commits/master)

Docker image of [Ark][] to use on a [Raspberry PI][].

Configure binfmt-support on the Docker host (works locally or remotely, i.e: using boot2docker):

    $ docker run --rm --privileged multiarch/qemu-user-static:register --reset

Then you can run an armhf image from your x86_64 Docker host :

    $ make run version=1.0

Or build :

    $ make build version=1.0


## License

See [LICENSE](LICENSE) for the complete license.


## Changelog

A [ChangeLog.md](ChangeLog.md) is available.


## Contact

Nicolas Lamirault <nicolas.lamirault@gmail.com>


[Raspberry PI]: https://www.raspberrypi.org/
[Ark]: https://github.com/heptio/ark
