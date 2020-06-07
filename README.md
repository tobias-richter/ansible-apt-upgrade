# tobias_richter.apt_upgrade

[![Build Status](https://travis-ci.org/tobias-richter/ansible-apt-upgrade.svg?branch=master)](https://travis-ci.org/tobias-richter/ansible-apt-upgrade)

This role performs an apt upgrade and cleans the apt cache afterwards.

## Requirements

This role requires Ansible 2.7 or higher.

## Role Variables

See [defaults/main.yml](defaults/main.yml) for the documented role variables.

## Example Playbook

This playbook executes a full apt upgrade.

    - hosts: apt_upgrade
	  roles:
	    - role: tobias_richter.apt_upgrade
	      apt_upgrade: "full"