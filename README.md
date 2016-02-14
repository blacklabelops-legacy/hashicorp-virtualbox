Container stuffed with Hashicorp Otto, Vagrant and Packer with Virtualbox!

Leave a message and ask questions on Hipchat: [blacklabelops/hipchat](https://www.hipchat.com/geogBFvEM)

Virtualbox base container with Hashicorp tool stack!

Requirements:

  * Centos7 dedicated host without any virtualization around.
  * Linux only, Virtualbox will not run inside Virtualbox or boot2docker!
  * Host machine must have working installation of Virtualbox.
  * Host machine should have same Virtualbox version.
  * Host machine should have same kernel version as container.

Software:

  * Virtualbox
  * Otto
  * Vagrant
  * Packer
  * Terraform
  * Atlas Upload Client

# Make It Short!

In short, you can use Otto, Vagrant and Packer and Virtualbox inside a Docker container!

~~~~
$ docker run --rm -it \
    --privileged=true \
    --device /dev/vboxdrv:/dev/vboxdrv \
    blacklabelops/virtualbox \
    bash
~~~~

> Mounts the hosts binaries. MUST use privileged mode, MUST mount host device.

# References

* [Docker Homepage](https://www.docker.com/)
* [Docker Userguide](https://docs.docker.com/userguide/)
* [Virtualbox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* [Packer](https://www.packer.io/)
