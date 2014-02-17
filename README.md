# Nagios NRPE Server Installation

[![Build Status](https://travis-ci.org/bobmaerten/ansible-role-nagios-nrpe-server.png?branch=master)](https://travis-ci.org/bobmaerten/ansible-role-nagios-nrpe-server)

Installs the Nagios NRPE agent and some custom checks on the target.

## Requirements

Currently only tested on Debian Wheezy 64


## Role Variables

Theses variables are defined by default, and can be overriden for this role:

    nagios_plugins_directory: /usr/lib/nagios/plugins
    nagios_server: centreon
    nagios_user: nagios
    nagios_group: nagios
    nrpe_port: 5666
    nrpe_pid_file: /var/run/nagios/nrpe.pid

You can and specify other template files for handling specific NRPE commands with:

    vars:
      nrpe_extra_commands:
        - <template>

And just put *template*.cfg files in the role template directory

## Usage

    ansible-galaxy install bobmaerten.nagios-nrpe-server

Also check the [Ansible Galaxy](https://galaxy.ansibleworks.com/intro) about page.


## License

MIT

## Author and other Information

By Bob Maerten

[GitHub project page](https://github.com/bobmaerten/ansible-role-nagios-nrpe-server)


