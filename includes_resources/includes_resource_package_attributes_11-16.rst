.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

This resource has the following properties:

``allow_downgrade``
   **Ruby Types:** TrueClass, FalseClass

   |resource yum_package| resource only. |allow_downgrade| Default value: ``false``.

``arch``
   **Ruby Types:** String, Array

   |resource yum_package| resource only. |architecture package|

``default_release``
   **Ruby Type:** String

   |resource package_apt| resource only. |default_release apt| For example: ``stable``.

``flush_cache``
   **Ruby Type:** Array

   |resource yum_package| resource only. |flush_cache| Default value: ``{ :before => false, :after => false }``.

   .. note:: |flush_cache yum_cache|

``gem_binary``
   **Ruby Type:** String

   |gem_binary resource package|

``ignore_failure``
   **Ruby Types:** TrueClass, FalseClass

   |ignore_failure| Default value: ``false``.

``notifies``
   **Ruby Type:** Symbol, 'Chef::Resource[String]'

   .. include:: ../../includes_resources_common/includes_resources_common_notification_notifies.rst

   .. include:: ../../includes_resources_common/includes_resources_common_notification_timers_12-5.rst

   .. include:: ../../includes_resources_common/includes_resources_common_notification_notifies_syntax.rst

``options``
   **Ruby Type:** String

   |command options|

``package_name``
   **Ruby Types:** String, Array

   |name package| |resource_block_default| |see syntax|

``provider``
   **Ruby Type:** Chef Class

   Optional. |provider resource_parameter| |see providers|

``response_file``
   **Ruby Type:** String

   |resource package_apt| and |resource package_dpkg| resources only. |response_file|

``response_file_variables``
   **Ruby Type:** Hash

   |resource package_apt| and |resource package_dpkg| resources only. |response_file variables|

``retries``
   **Ruby Type:** Integer

   |retries| Default value: ``0``.

``retry_delay``
   **Ruby Type:** Integer

   |retry_delay| Default value: ``2``.

``source``
   **Ruby Type:** String

   Optional. |source resource package|

``subscribes``
   **Ruby Type:** Symbol, 'Chef::Resource[String]'

   .. include:: ../../includes_resources_common/includes_resources_common_notification_subscribes.rst

   .. include:: ../../includes_resources_common/includes_resources_common_notification_timers_12-5.rst

   .. include:: ../../includes_resources_common/includes_resources_common_notification_subscribes_syntax.rst

``timeout``
   **Ruby Types:** String, Integer

   |timeout|

``version``
   **Ruby Types:** String, Array

   |version package|
