## Docker Dev

A simple [Vagrant][1] and [Ansible][2] project to stand up a [Docker][3]
development environment. Includes `docker-compose`. The box is based on
[Debian Jessie][5] because it's [free][6] and awesome.

You can also use this to learn a little bit about [Vagrant][1] and Ansible[2].

## Use

Make sure you've [installed Vagrant][4].

From the project directory, containing the `Vagrantfile`, run:

    vagrant up

wait a bit. (It can take a while to update Debian, install Docker, etc.) For example:

    $ time vagrant up
    ...
    real	22m47.561s
    user	0m44.163s
    sys	    0m4.643s

Then:

    vagrant ssh

From the Vagrant box:

    docker -v

use docker _for great justice!_

## How?

There is a standard, simple, and commented set of Ansible files in the
`provisioning` directory.

## Watch

[![asciicast](https://asciinema.org/a/mKOjemRqoPN3JZ65I5dqs9LfS.png)](https://asciinema.org/a/mKOjemRqoPN3JZ65I5dqs9LfS)

## Testing

Tested using the following versions

| [Vagrant][1] | [Virtual Box][7]   | Vagrant Plugins |
| :---         | :---               | :---            |
| 2.0.2   | 5.2.6 r120293 (Qt5.9.1) | vagrant-cachier (1.2.1), vagrant-vbguest (0.15.1) ||


<!-- refs -->
[1]: https://www.vagrantup.com "Vagrant"
[2]: http://docs.ansible.com/ansible/index.html "Ansible docs"
[3]: https://docker.com "Docker"
[4]: https://www.vagrantup.com/docs/installation/ "Vagrant installation"
[5]: https://www.debian.org "Debian The Universal Operating System"
[6]: https://www.debian.org/intro/free "Freedom"
[7]: https://www.virtualbox.org/
