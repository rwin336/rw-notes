# Problem Description

The docker_container ansible module requires ansible version 2.1.0 or greater.  The baseline Ubuntu Xenial 16.04 comes with 2.0.0.2.  Therefore the need to upgrade

# Platform:  
Ubuntu Xenial 16.04


# Procedure:
1. Review installation reference(http://docs.ansible.com/ansible/intro_installation.html)
2. Remove ansible 2.0.0.2
   * sudo apt-get remove ansible
3. Goto the Ansible Download (http://releases.ansible.com/ansible/) and pick the release you want
   * ansible-latest.tar.gz
4. Make a direcotry /opt/ansible and set world rwx privs
5. Copy ansible tarball to /opt/ansible
6. Unzip and untar
7. cd to the ansible-2.x.x.x directory
8. As sudo run the setup.py
   * sudo python ./setup.py install 
9. Verify with ansible --version


# Docker.py 
Since the goal of upgrading ansible is to use ansible's docker_container module make sure it is installed.

sudo pip install docker.py
  

