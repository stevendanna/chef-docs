.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

The |resource deploy| resource expects an application to be structured like a |ruby on rails| application, but the layout can be modified to meet custom requirements as needed. Use the following attributes to specify custom application layouts within a recipe:

* ``create_dirs_before_symlink``
* ``purge_before_symlink``
* ``symlinks``
* ``symlink_before_migrate``
