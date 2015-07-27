## crypttab

[![Travis CI](http://img.shields.io/travis/ypid/ansible-crypttab.svg?style=flat)](http://travis-ci.org/ypid/ansible-crypttab)
[![Ansible Galaxy](http://img.shields.io/badge/galaxy-ypid.crypttab-660198.svg?style=flat)](https://galaxy.ansible.com/list#/roles/4559)
[![Platforms](http://img.shields.io/badge/platforms-debian%20/%20ubuntu-lightgrey.svg?style=flat)](#)


Manage cryptsetup devices via /etc/crypttab.

In case you need to copy keyfiles to the target you might want to checkout the [copy role][].

### Features

* Add or remove devices in /etc/crypttab
* Optionally add or remove these devices in /etc/fstab

[copy role]: https://galaxy.ansible.com/list#/roles/4558

### Installation

This role requires at least Ansible `v1.8.4`. To install it, run:

    ansible-galaxy install ypid.crypttab

To install via git, run either:

    git clone https://github.com/ypid/ansible-crypttab.git ypid.crypttab
    git submodule add https://github.com/ypid/ansible-crypttab.git roles/ypid.crypttab




### Role variables

List of default variables available in the inventory:

    ---
    
    # "Global" crypttab devices
    crypttab_list:
    
    # "Host group" crypttab devices
    crypttab_group_list:
    
    # "Host" crypttab devices
    crypttab_host_list:
      # - name: 'luks-home'
      #   backing_device: 'UUID=bb51423a-3384-11e5-beee-3cd92b26fd34'
      #   password: '/path/to/keyfile'
    
    # crypttab_default_options: 'discard'




### Authors and license

`crypttab` role was written by:

- [Robin Schneider](https://github.com/ypid) | [e-mail](mailto:ypid@riseup.net)

License: [AGPLv3](https://tldrlegal.com/license/gnu-affero-general-public-license-v3-%28agpl-3.0%29)

***

README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).
