# tomcat9-standalone_ansible

This ansible script install on remote machine The Tomcat application server 9 and enabling management console to manage it

N.B.

Oracle Jdk it is not installed.  The user will have to install it through rpm package or tar.gz and afterwards setting JAVA_HOME

However this ansible is tested with Oracle jdk 10.1

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
epel

For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
