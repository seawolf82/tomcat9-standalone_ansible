# tomcat9-standalone_ansible

This ansible script install on remote machine The Tomcat application server 9

N.B.

Oracle Jdk it is not installed.  The user will have to install it through rpm package ora tar.gz ans afterwards setting JAVA_HOME

To launch ansible script use:

ansible-playbook -vv -i hosts site.yaml
