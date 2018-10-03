# RPI Kubernetes ExternalDNS

* Master: [![pipeline status](https://gitlab.com/zeiot/rpi-external-dns/badges/master/pipeline.svg)](https://gitlab.com/zeiot/rpi-external-dns/commits/master)

Docker image of [Kubernetes external-dns][] to use on a ARM(64) device.

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


[external-dns]: https://github.com/kubernetes-incubator/external-dns
