# Coolify IaC provisioning
This project tries to figure out possibilities to configure coolify in a reproducable fashion.
The Project assumes you have a coolify installation running on some host.
To easily met this assumption it provides a Vagrant box providing a fresh coolify installation

## Development
To simulate the assumption you having a running coolify instance we spin one up via vagrant.
> The Vagrant setup is compatible with MacOS silicon machines. Other host OS/setups hasn't been tested and are out of interest for this project.

After spinning up the coolify VM it will be available at http://localhost:8000

### Requirements
#### vagrant installed
    brew install --cask vagrant vagrant-manager vmware-fusion vagrant-vmware-utility
    vagrant plugin install vagrant-vmware-desktop

#### terraform installed
    brew install terraform

### How-To
#### spin-up coolify VM
    vagrant up

#### reload VM config (Vagrantfile)
    vagrant reload

#### ssh into VM
    vagrant ssh

#### destroy VM
    vagrant destroy