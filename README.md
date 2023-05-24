Docker Ubuntu Systemd
=====================

This Dockerfile can build containers capable to use systemd and sudo. Its a fork of Robert deBock with sudo added.

[![build-push](https://github.com/othiman/docker-ubuntu-systemd/actions/workflows/build-push-action.yml/badge.svg)](https://github.com/othiman/docker-ubuntu-systemd/actions/workflows/build-push-action.yml)

Branches
--------

This repository use branches that relate to Ubuntu a version.

|Branch |Ubuntu Version        |Docker image tag|
|-------|----------------------|----------------|
|master |jammy (22.04)         |latest          |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  schlien/ubuntu-ansible-systemd
```
