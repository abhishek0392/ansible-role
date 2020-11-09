# Ansible role to install groovy .

This role will install groovy and set the GROOVY_HOME path.


## Role Variables



groovy_version: "2.4.10"
- Groovy version you want to install . Default version - 2.4.10

groovy_base: /usr/local/src/groovy
- Set the groovy base path

groovy_home: "{{ groovy_base }}/latest"
groovy_home_script_name: groovy.sh

groovy_directory: "{{ groovy_base }}/groovy-{{ groovy_version }}"
groovy_download: https://bintray.com/artifact/download/groovy/maven/apache-groovy-binary-{{ groovy_version }}.zip


groovy_owner: root
groovy_group: "{{ groovy_owner }}"

