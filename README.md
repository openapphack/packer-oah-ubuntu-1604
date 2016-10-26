# OAH Ubuntu 16.04 minimal Vagrant Box

**Ubuntu Version Used**: 16.04.1

This build configuration installs and configures Ubuntu 16.04 x86_64 minimal using Ansible, and then generates a vagrant box for VirtualBox

## Requirements

The following software must be installed/present on your local machine:

  - [Packer](http://www.packer.io/)
  - [Vagrant](http://vagrantup.com/)
  - [VirtualBox](https://www.virtualbox.org/)
  - [Ansible](http://docs.ansible.com/intro_installation.html)

Install the ansible roles if not already installed required using :

  1. Run `$ ansible-galaxy install -r requirements.yml` in this directory.
  2. If your local Ansible roles path is not the default (`/etc/ansible/roles`), update the `role_paths` inside `oahubuntu1604.json` to match your custom location.

## Usage

    $ packer build oahubuntu1604.json

After sometime, Packer should tell you the box was generated successfully.

## License

MIT license.
