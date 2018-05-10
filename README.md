# Ansible Role: deploy-war-in-websphere-libertyy-core

An Ansible Role that deploy a war/jar application on Websphere Liberty core.

## Requirements

* Download the latest version of wlp-featureRepo from http://www-01.ibm.com/support and put it on `/YourWorkspace/docker_files/websphere`
* edit the version in the `templates/dockerfile-Liberty-Core.j2`

## Role Variables

**WarApps** : A list of applications.
* name : name of the project
* path_to_war : the path that contain your war/jar application
* libs : list of libraries

      base_path_linux: /opt/livrables

the default path where to save (Dockerfile, server.xml and app.war)


## Example Playbook
```
    - hosts: all
      roles:
        - ansible-role-deploy-war-in-websphere-liberty

```
## License

HACH

## Author Information

This role was created in 2018 by [Hakim CHRIFI ALAOUI](https://github.com/Hakimo003/ansible-role-deploy-war-in-websphere-liberty).
