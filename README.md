# tomcat9-standalone_ansible

This ansible script install on remote machine The Tomcat application server 9 and enabling management console to manage it

N.B.

Oracle Jdk it is not installed.  The user will have to install it through rpm package or tar.gz and afterwards setting JAVA_HOME

However this ansible is tested with Oracle jdk 10.1

To install tomcat run:

ansible-playbook -vv -i hosts site.yaml

To uninstall tomcat run:

ansible-playbook -vv -i hosts deprovision.yaml
