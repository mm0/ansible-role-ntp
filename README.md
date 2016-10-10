# README.md

# Ansible Role: NTP v1.0

An Ansible role that installs and re-configures NTP daemon with your list of servers

See Also: ansible-role-directory

![travis-ci](https://travis-ci.org/mm0/ansible-role-ntp.svg?branch=master)

## Requirements

None 

## Role Variables

Available variables are listed below, along with values defaults to AWS servers:

    ntp_servers: 
		- server 0.amazon.pool.ntp.org iburst
		- server 1.amazon.pool.ntp.org iburst
		- server 2.amazon.pool.ntp.org iburst
		- server 3.amazon.pool.ntp.org iburst

## Dependencies

None 

## Example Playbook

    - hosts: webservers
      roles:
      - { role: ansible-role-ntp }

## License

MIT
