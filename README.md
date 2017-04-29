Debian-Kibana
=============

Visualize logs and time-stamped data. Elasticsearch works seamlessly with Kibana to let you see and interact with your data.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

kibana:
    version: 3.1.1
    url : https://download.elasticsearch.org/kibana/kibana/kibana-3.1.1.zip
    destination: /var/www

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-kibana, kibana.version: 3.1.1, kibana.url : https://download.elasticsearch.org/kibana/kibana/kibana-3.1.1.zip, kibana.destination: /var/www }

Tasks
-----

  - Install [Kibana](http://www.elasticsearch.org/overview/kibana/) tool

License
-------

BSD
