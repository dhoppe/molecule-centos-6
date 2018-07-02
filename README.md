# CentOS image for Molecule

This [Docker](https://www.docker.com) image can be used to test [Ansible](https://www.ansible.com) playbooks based on [Molecule](https://molecule.readthedocs.io/en/latest/).

## Supported tags

* latest
* 6

## Usage

Run the container as a daemon

```console
docker run --cap-add SYS_ADMIN --detach --name centos-6 --rm --volume /sys/fs/cgroup:/sys/fs/cgroup:ro dhoppe/molecule-centos-6
```

Enter the container

```console
docker exec -it centos-6 bash
```

Stop the container

```console
docker stop centos-6
```