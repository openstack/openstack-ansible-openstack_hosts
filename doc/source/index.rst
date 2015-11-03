OpenStack_hosts Role Docs
=========================

Role for basic setup and configuration of a host machine for the intended purpose of
use within OpenStack. This role was created to tune a host to receive OpenStack.
The basic operations within the role allow it to install, setup, and tune specific
kernel options that all OpenStack powered hosts will need to perform nominally.


Basic Role Example
^^^^^^^^^^^^^^^^^^

.. code-block:: yaml

    - name: Basic host setup
      hosts: "hosts"
      user: root
      roles:
        - { role: "openstack_hosts", tags: [ "openstack-hosts-setup" ] }
