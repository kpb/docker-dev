## Docker Dev

A simple [Vagrant][1] and [Ansible][2] project to stand up a [Docker][3]
development environment. Includes `docker-compose`.

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


[1]: https://www.vagrantup.com "Vagrant"
[2]: http://docs.ansible.com/ansible/index.html "Ansible docs"
[3]: https://docker.com
[4]: https://www.vagrantup.com/docs/installation/ "Vagrant installation"
