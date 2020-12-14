# tobias_richter.apt_upgrade

[![Build Status](https://github.com/tobias-richter/ansible-apt-upgrade/workflows/CI/badge.svg)](https://github.com/tobias-richter/ansible-apt-upgrade/actions)

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