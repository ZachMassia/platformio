..  Copyright 2014-2016 Ivan Kravets <me@ikravets.com>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _envvars:

Environment variables
=====================

`Environment variables <http://en.wikipedia.org/wiki/Environment_variable>`_
are a set of dynamic named values that can affect the way running processes
will behave on a computer.

*PlatformIO* handles variables which start with ``PLATFORMIO_`` prefix. They
have the **HIGHEST PRIORITY**.

.. contents::

General
-------

PlatformIO uses *General* environment variables for the common
operations/commands.

.. envvar:: CI

PlatformIO handles ``CI`` variable which is setup by
`Continuous Integration <http://en.wikipedia.org/wiki/Continuous_integration>`_
(Travis, Circle and etc.) systems.
Currently, PlatformIO uses it to disable prompts.

In other words, ``CI=true`` automatically setup
:envvar:`PLATFORMIO_SETTING_ENABLE_PROMPTS=false <PLATFORMIO_SETTING_ENABLE_PROMPTS>`.

.. envvar:: PLATFORMIO_HOME_DIR

Allows to override :ref:`projectconf` option :ref:`projectconf_pio_home_dir`.

.. envvar:: PLATFORMIO_LIB_DIR

Allows to override :ref:`projectconf` option :ref:`projectconf_pio_lib_dir`.

.. envvar:: PLATFORMIO_SRC_DIR

Allows to override :ref:`projectconf` option :ref:`projectconf_pio_src_dir`.

.. envvar:: PLATFORMIO_ENVS_DIR

Allows to override :ref:`projectconf` option :ref:`projectconf_pio_envs_dir`.

.. envvar:: PLATFORMIO_DATA_DIR

Allows to override :ref:`projectconf` option :ref:`projectconf_pio_data_dir`.


Builder
-------

.. envvar:: PLATFORMIO_BUILD_FLAGS

Allows to set :ref:`projectconf` option :ref:`projectconf_build_flags`.

.. envvar:: PLATFORMIO_SRC_BUILD_FLAGS

Allows to set :ref:`projectconf` option :ref:`projectconf_src_build_flags`.

.. envvar:: PLATFORMIO_SRC_FILTER

Allows to set :ref:`projectconf` option :ref:`projectconf_src_filter`.

.. envvar:: PLATFORMIO_EXTRA_SCRIPT

Allows to set :ref:`projectconf` option :ref:`projectconf_extra_script`.


Settings
--------

Allows to override PlatformIO settings. You can manage them via
:ref:`cmd_settings` command.

.. envvar:: PLATFORMIO_SETTING_AUTO_UPDATE_LIBRARIES

Allows to override setting :ref:`setting_auto_update_libraries`.

.. envvar:: PLATFORMIO_SETTING_AUTO_UPDATE_PLATFORMS

Allows to override setting :ref:`setting_auto_update_platforms`.

.. envvar:: PLATFORMIO_SETTING_CHECK_LIBRARIES_INTERVAL

Allows to override setting :ref:`setting_check_libraries_interval`.

.. envvar:: PLATFORMIO_SETTING_CHECK_PLATFORMIO_INTERVAL

Allows to override setting :ref:`setting_check_platformio_interval`.

.. envvar:: PLATFORMIO_SETTING_CHECK_PLATFORMS_INTERVAL

Allows to override setting :ref:`setting_check_platforms_interval`.

.. envvar:: PLATFORMIO_SETTING_ENABLE_PROMPTS

Allows to override setting :ref:`setting_enable_prompts`.

.. envvar:: PLATFORMIO_SETTING_ENABLE_TELEMETRY

Allows to override setting :ref:`setting_enable_telemetry`.
