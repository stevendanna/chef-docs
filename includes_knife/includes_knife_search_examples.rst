.. The contents of this file are included in multiple topics.
.. This file describes a command or a sub-command for Knife.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.


For example, to search for the IDs of all nodes running on the |amazon ec2| platform, enter:

.. code-block:: bash

   $ knife search node 'ec2:*' -i

to return something like:

.. code-block:: bash

   4 items found
   
   ip-0A7CA19F.ec2.internal
   
   ip-0A58CF8E.ec2.internal
   
   ip-0A58E134.ec2.internal
   
   ip-0A7CFFD5.ec2.internal

To search for the instance type (flavor) of all nodes running on the |amazon ec2| platform, enter:

.. code-block:: bash

   $ knife search node 'ec2:*' -a ec2.instance_type

to return something like:

.. code-block:: bash

   4 items found
   
   ec2.instance_type:  m1.large
   id:                 ip-0A7CA19F.ec2.internal
   
   ec2.instance_type:  m1.large
   id:                 ip-0A58CF8E.ec2.internal
   
   ec2.instance_type:  m1.large
   id:                 ip-0A58E134.ec2.internal
   
   ec2.instance_type:  m1.large
   id:                 ip-0A7CFFD5.ec2.internal

To search for all nodes running |ubuntu|, enter:

.. code-block:: bash

   $ knife search node 'platform:ubuntu'

To search for all nodes running |centos| in the production environment, enter:

.. code-block:: bash

   $ knife search node 'chef_environment:production AND platform:centos'

