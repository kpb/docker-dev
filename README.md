## Docker Dev

A simple [Vagrant][1] and [Ansible][2] project to stand up a [Docker][3]
development environment. Includes `docker-compose`. The box is based on
[Debian Jessie][5] because it's [free][6] and awesome.

## Use

Make sure you've [installed Vagrant][4].

From the project directory, containing the `Vagrantfile`, run:

    vagrant up

wait a bit. Then:

    vagrant ssh

From the Vagrant box:

    docker -v

use docker _for great justice!_

## How?

There is a standard, simple, and commented set of Ansible files in the
`provisioning` directory.

## Look

<script type="text/javascript" src="https://asciinema.org/a/mKOjemRqoPN3JZ65I5dqs9LfS.js" id="asciicast-mKOjemRqoPN3JZ65I5dqs9LfS" async></script>

<!-- refs -->
[1]: https://www.vagrantup.com "Vagrant"
[2]: http://docs.ansible.com/ansible/index.html "Ansible docs"
[3]: https://docker.com
[4]: https://www.vagrantup.com/docs/installation/ "Vagrant installation"
[5]: https://www.debian.org "Debian The Universal Operating System"
[6]: https://www.debian.org/intro/free "Freedom"
