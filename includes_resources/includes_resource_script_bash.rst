.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

Use the |resource script_bash| resource to execute scripts using the |bash| interpreter. This resource may also use any of the actions and properties that are available to the |resource execute| resource. Commands that are executed with this resource are (by their nature) not idempotent, as they are typically unique to the environment in which they are run. Use ``not_if`` and ``only_if`` to guard this resource for idempotence.

.. note:: The |resource script_bash| script resource (which is based on the |resource script| resource) is different from the |resource ruby_block| resource because |ruby| code that is run with this resource is created as a temporary file and executed like other script resources, rather than run inline. 
