# sol1-powerdns-lightningstream
Ansible Role to install PowerDNS Lightning Stream.

This role installs the lightning stream package, adds lightning stream configuration and a system service.

## Dependancy
The lightning stream package is installed on debain from packages.sol1.net. The apt repository for this is installed via a dependant role `sol1.packages_repo` which is maintained at https://github.com/sol1-ansible/sol1-packages_repo.

Add this to `roles/requirements.yml`
```
- name: sol1.packages_repo
  src: git+https://github.com/sol1-ansible/sol1-packages_repo
  version: main
```  
