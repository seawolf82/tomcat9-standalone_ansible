# tomcat9-standalone_ansible

This ansible script install on remote machine The Tomcat application server 9 and enabling management console to manage it

Tested with openjdk17 on Almalinux8-9 RockyLinux8-9

Tested with openjdk18 on Centos7

To install tomcat run:

ansible-playbook -vv -i hosts site.yaml

To uninstall tomcat run:

ansible-playbook -vv -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
selinux
ntp
tomcat

For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
