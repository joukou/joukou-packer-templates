Joukou Packer Templates
=======================
[![Apache 2.0](http://img.shields.io/badge/License-Apache%202.0-brightgreen.svg)](#license) [![Stories in Ready](https://badge.waffle.io/joukou/joukou-packer-templates.png?label=ready&title=Ready)](http://waffle.io/joukou/joukou-packer-templates) [![IRC](http://img.shields.io/badge/IRC-%23joukou-blue.svg)](http://webchat.freenode.net/?channels=joukou)

These templates build the Vagrant box files used for development on virtual
machines such as VirtualBox and VMware Fusion. You should not need to ever use
this repository unless you are updating or modifying the development box files.

## Usage

1. Download and Install [Vagrant](http://www.vagrantup.com/)
1. Download and Install [VMware Fusion](http://www.vmware.com/products/fusion/)
  - License(s) on Google Drive under `Joukou/Technology/Licenses/VMware Fusion`
1. Download and Install the [Vagrant VMware Fusion Provider](https://www.vagrantup.com/vmware)
  - License on Google Drive under `Joukou/Technology/Licenses/Vagrant`
1. Download and Install [VirtualBox](https://www.virtualbox.org/)
1. Download and Install [Packer](http://www.packer.io/)
1. `packer build template.json`
1. Upload the built `*.box` files to Amazon S3 to the `joukou` bucket. Use the
   existing `vagrant` folder structure.
1. If the box already exists under the Joukou organisation on [Vagrant Cloud](https://vagrantcloud.com);
  1. Add a new version to the existing box
  1. Use the S3 URL instead of Upload for the box files
1. If the box does not already exist under the Joukou organisation;
  1. Create a new public box
  1. Use the S3 URL instead of Upload for the box files

## License

Copyright &copy; 2014 Joukou Ltd.

Joukou Packer Templates is under the Apache 2.0 license. See the
[LICENSE](LICENSE) file for details.