# Infra Utils

**An Ansible Playbook to install and configure the containers I use within my home infrastructure.**
Currently:
* [pi-hole](https://pi-hole.net)
* [grafana](https://grafana.com)
* [prometheus](https://prometheus.io)
* [speedtest-exporter](https://github.com/MiguelNdeCarvalho/speedtest-exporter) for prometheus
* [blackbox-exporter](https://github.com/prometheus/blackbox_exporter) for prometheus for ping tracking

## Background 
The initial plan was to take [Jeff Geerling](https://www.jeffgeerling.com)'s [internet-pi](https://github.com/geerlingguy/internet-pi) project and simply convert it for use on EL-based linuxes ([Fedora](https://getfedora.org), [CentOS Stream](https://www.centos.org/centos-stream/), [RHEL](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux), etc) and to use [podman](https://podman.io) instead of docker (see [Considerations](#considerations) for details).  Turned out the latter was more complicated that I had originally thought since I was planning on leveraging rootless-containers in podman for enhanced security and Jeff's original docker design used rootful containers extensively.  So I rebuilt it from scratch.

## Features
COMING SOON

## Considerations
COMING SOON

## Links
Here's a list (in no particular order) to sites that helped me through some of my design or implementation snafus: 
* https://discourse.pi-hole.net/t/setup-pihole-using-rootless-podman-and-ansible/46414
* https://fedoramagazine.org/podman-with-capabilities-on-fedora/
* https://jreypo.io/2021/03/12/running-pihole-as-a-podman-container-in-fedora/
* https://github.com/ikke-t/ansible-podman-examples/blob/d51d5efa0d41744111b9484f7adea759cdfeeb59/run-container-pihole-podman.yml
* https://redhatnordicssa.github.io/grafana-rootless-container-ansible
* https://www.tutorialworks.com/podman-rootless-volumes/
* https://blog.while-true-do.io/podman-volumes-1/