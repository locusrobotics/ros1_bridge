^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package ros1_bridge
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.7.0 (2019-03-18)
------------------
* Tailor: Updating Jenkinsfile
* Misc Improvements (`#1 <https://github.com/locusrobotics/ros1_bridge/issues/1>`_)
  * Add wait to ROS1 server and improve logging
  * Fixup logging
* Tailor: Updating Jenkinsfile
* Tailor: Updating Jenkinsfile
* Tailor: Creating Jenkinsfile
* Allow latching for ROS1 pub, and custom qos for ROS2 components
* Allow external use of ros1_bridge library factories
* 0.6.1
* exclude ros1 nodelets (`#152 <https://github.com/locusrobotics/ros1_bridge/issues/152>`_)
  * exclude ros1 nodelets
  * find_package() only if neccessary
  * add todo
* fix is_package_mapping check (`#151 <https://github.com/locusrobotics/ros1_bridge/issues/151>`_)
* 0.6.0
* expose convert function (`#146 <https://github.com/locusrobotics/ros1_bridge/issues/146>`_)
  * expose convert function
  * expose convert2_to_1 function
  * export roscpp as dependency
  * Revert "export roscpp as dependency"
  This reverts commit d8a1ccc25c8d7811c6148ce2a5ff6920c16188a9.
* support for custom field mapping for services (`#147 <https://github.com/locusrobotics/ros1_bridge/issues/147>`_)
  * support for custom field mapping for services
  * Update doc/index.rst
  Co-Authored-By: dirk-thomas <dirk-thomas@users.noreply.github.com>
* handle idl files correctly (`#145 <https://github.com/locusrobotics/ros1_bridge/issues/145>`_)
* Fix for actions subfolder introduction in ros2 message bridge (`#143 <https://github.com/locusrobotics/ros1_bridge/issues/143>`_)
  * Fix for actions subfolder introduction in ros2 message bridge
  * Updating service_name for action srvs for compatibility
  * Extended changes on ros1_bridge
  * Undo of action specific locations to ros1_bridge
  * lint fixup
* use new error handling API from rcutils (`#141 <https://github.com/locusrobotics/ros1_bridge/issues/141>`_)
  Signed-off-by: William Woodall <william@osrfoundation.org>
* changed cmake message logger level (`#138 <https://github.com/locusrobotics/ros1_bridge/issues/138>`_)
* 0.5.1
* update doc to reflect that any mapping combination is supported
* rule can be a message mapping even if a field mapping is provided as well (`#135 <https://github.com/locusrobotics/ros1_bridge/issues/135>`_)
* 0.5.0
* remove --build-tests which is an ament argument from colcon invocation
* print service pairs as well (`#124 <https://github.com/locusrobotics/ros1_bridge/issues/124>`_)
  * print service pairs as well
  * add variable to template header
* print message for all ROS 2 message pkgs (`#123 <https://github.com/locusrobotics/ros1_bridge/issues/123>`_)
* update README to use colcon and ROS Melodic (`#122 <https://github.com/locusrobotics/ros1_bridge/issues/122>`_)
  * update README to use colcon and ROS Melodic
  * clarify MAKEFLAGS is an env var
* include module name which wasn't found in error message (`#121 <https://github.com/locusrobotics/ros1_bridge/issues/121>`_)
* use catkin_pkg to parse packages (`#119 <https://github.com/locusrobotics/ros1_bridge/issues/119>`_)
  * ament_package doesnt provide parse_package anymore
  * python3 version of catkin_pkg is now ensured to be available
* migrate launch -> launch.legacy (`#117 <https://github.com/locusrobotics/ros1_bridge/issues/117>`_)
* Duplicate messages in bidirectional_bridge fix (`#113 <https://github.com/locusrobotics/ros1_bridge/issues/113>`_)
  * Pass ros2_publisher to ros2_subscriber callback
  * Pass message_info to ros2_subscriber callback
  * Add gid compare to ignore messages from bridge itself
  * Fix style issues to pass tests
  * Edit comment
  * Add else statement to raise an exception and reset rmw error
  * Fix cpplint and uncrustify failures
* Fix linter failures from includes (`#110 <https://github.com/locusrobotics/ros1_bridge/issues/110>`_)
  * Fix linter failures from includes
  * reorder
  * Alphabetical order was fine how it was
* Map duration and time messages (`#106 <https://github.com/locusrobotics/ros1_bridge/issues/106>`_)
  * add missing dependencies
  * change variable name since the argument is not a message but a type
  * custom handling of builtin_interfaces to provide mapping to std_msgs
* clarify that all field must be listed explicitly (`#109 <https://github.com/locusrobotics/ros1_bridge/issues/109>`_)
* add an error message if the mapping rules are not a list (`#107 <https://github.com/locusrobotics/ros1_bridge/issues/107>`_)
* advise to ask questions on ROS answers
* 0.4.0
* match topic name printed in console (`#102 <https://github.com/locusrobotics/ros1_bridge/issues/102>`_)
* Update for rclcpp namespace removals (`#101 <https://github.com/locusrobotics/ros1_bridge/issues/101>`_)
  * Remove ::publisher:: namespace
  * Remove subscription:: namespace
  * Remove client:: namespace
  * Remove service:: namespace
  * Remove node:: namespace
  * Remove utilities:: namespace
* cmake 3.10 compatibility: pass absolute path to file(GENERATE) function (`#100 <https://github.com/locusrobotics/ros1_bridge/issues/100>`_)
* depend on rosidl_interfaces_packages group (`#99 <https://github.com/locusrobotics/ros1_bridge/issues/99>`_)
  * depend on rosidl_interfaces_packages group
  * typo
  * rosidl_interfaces_packages -> rosidl_interface_packages
* Fix building of ros1_bridge against newer roscpp. (`#98 <https://github.com/locusrobotics/ros1_bridge/issues/98>`_)
  The comment in the code mostly explains it, but because of changes
  to upstream catkin/roscpp, we need to expand the types of things
  we look at for linking.  With this patch, building against
  roscpp kinetic 1.12.7 and 1.12.12 works.
  Signed-off-by: Chris Lalancette <clalancette@osrfoundation.org>
* use ament_cmake_pytest instead of ament_cmake_nose
* print bridged type names
* Increase timeout waiting for server for ros2 client in tests (`#94 <https://github.com/locusrobotics/ros1_bridge/issues/94>`_)
* update style to match latest uncrustify (`#93 <https://github.com/locusrobotics/ros1_bridge/issues/93>`_)
* 0.0.3
* only show a message for passing the message of a specific type pair once
* remove check for header fields request_type and response_type
* add missing dependencies in readme (`#89 <https://github.com/locusrobotics/ros1_bridge/issues/89>`_)
  * add missing dependencies in readme
  * add space between ROS 1
* update style to satisfy new flake8 plugins (`#87 <https://github.com/locusrobotics/ros1_bridge/issues/87>`_)
* implicitly inherit from object (`#86 <https://github.com/locusrobotics/ros1_bridge/issues/86>`_)
* add issue template
* note about memory (`#85 <https://github.com/locusrobotics/ros1_bridge/issues/85>`_)
  * note about memory
  * Update README.md
  * Update README.md
* Readme fixups (`#83 <https://github.com/locusrobotics/ros1_bridge/issues/83>`_)
  * even on SBCs build can be built with j2 since the bridge refactor
  * force cmake on bridge building invocation
* more ros2 run
* use ros2 run
* 0.0.2
* The python yaml module is needed for ros1_bridge_generate_factories (`#80 <https://github.com/locusrobotics/ros1_bridge/issues/80>`_)
* Fix fd leak (`#79 <https://github.com/locusrobotics/ros1_bridge/issues/79>`_)
  * Fix the constantly leaking fd's in the dynamic_bridge.
  * fix style making uncrustify complain
  * Capture transport by value.
* use rosrun API to determine talker/listener path
* install executables in package specific path
* handle multiple types per topic (`#73 <https://github.com/locusrobotics/ros1_bridge/issues/73>`_)
  * handle multiple types per topic
  * fix ros1 service client -> ros2 service server
* use CMAKE_X_STANDARD and check compiler rather than platform
* rename variable to not use underscore prefix
* Find ROS1 message packages (`#67 <https://github.com/locusrobotics/ros1_bridge/issues/67>`_)
  * rename message_packages variable
  * find ros1 message packages
  * fail hard with explicit error message if rosmsg/rossrv failed to run
  * ensure only ros1 message packages on pythonpath when running rosmsg/rossrv
  * refactor
  * still need to convert to path using : delimiter on UNIX machines
* Fix topic matching (`#71 <https://github.com/locusrobotics/ros1_bridge/issues/71>`_)
  * do not truncate leading / when listing ROS 1 topics
  * do not leave partial key when service info is incomplete
  * style fix
* add parameter-based bridge
* Call is\_*_mapping functions instead of treating them as booleans (`#70 <https://github.com/locusrobotics/ros1_bridge/issues/70>`_)
* fix race conditions
* add missing trailing newlines
* check for substrings before using their iterator
* add option to dynamic_bridge to print out message type pairs (`#59 <https://github.com/locusrobotics/ros1_bridge/issues/59>`_)
  * add --print-pairs option to dynamic_bridge
  This prints a list of ROS 2 <=> ROS 2 message type conversion pairs that were built into the bridge.
  * add a hint to stderr when a pair is not found
  * typo
* Fixed crashing discovery of ROS2 services (`#58 <https://github.com/locusrobotics/ros1_bridge/issues/58>`_)
* correctly export libraries and fix LD_LIB path (`#57 <https://github.com/locusrobotics/ros1_bridge/issues/57>`_)
* fix import order
* remove unnecessary include
* use rmw implementation
* dependency order
* require CMake 3.5
* replace deprecated <CONFIGURATION> with <CONFIG>
* Use std chrono literals (`#52 <https://github.com/locusrobotics/ros1_bridge/issues/52>`_)
  * update references to rclcpp_tutorials to be demo_nodes_cpp
  * use std chrono literals
* update references to rclcpp_tutorials to be demo_nodes_cpp (`#51 <https://github.com/locusrobotics/ros1_bridge/issues/51>`_)
* replace custom test with launch based test for msg and srv
* cleanup and pass all linters
* Rework after the review (`#36 <https://github.com/locusrobotics/ros1_bridge/issues/36>`_)
  * Removed separate file for mapping services
  * Other minor changes
* Add option for bridging all topics (`#42 <https://github.com/locusrobotics/ros1_bridge/issues/42>`_)
  * Refactor "Create ros2->1 bridge" logic
  * Bridge ROS 2 to ROS 1 even if no ROS 1 listeners
  * Only print warning if it's not a forced bridge
  * Expose command-line options for bridge-all-topics
  * Mention new options in readme
  * Revert "Only print warning if it's not a forced bridge"
  This reverts commit 2ca07796bec71fc3c381b55a06e4bd72c23bf151.
  * lint
  * Check if there's a mapping before forcing bridge
  * No need to support empty typenames for ROS 2 anymore
  * Move get_xtox_mapping methods to their own file
  * avoid unnecessary whitespace changes
  * Add missing template
  * Update from review
  * lint
  * Only pass the relevant data to the template
* c++14 (`#46 <https://github.com/locusrobotics/ros1_bridge/issues/46>`_)
* Change ROS 2 publishers to reliable so any reliability profile can connect (`#37 <https://github.com/locusrobotics/ros1_bridge/issues/37>`_)
  * Change ROS 2 publishers to reliable so any reliability profile can connect
  * No need for custom talker + listener anymore
  * Update from review
  * rclcpp_examples -> rclcpp_tutorials
* Bridging services (`#36 <https://github.com/locusrobotics/ros1_bridge/issues/36>`_)
  * Added support for bridging services
  * Added tests and fixes after the review
  - printing errors to stderr
  - replaced boost library with std
  - fixed indentation in templates
  - support for a manual service matching
  - simplified an example in README
  * Fixed issues after a review
  - Service factory does not raise errors anymore
  - Handling exceptions while creating/removing bridges
  - Fixed syntax in index.rst
  * Updated services to use separate compilation units
* remove leftover sentence
* Add mention to tf2_msgs
* Be more explicit about the reason we're adding packages to the path
* Update from review
* generate package specific compilation units
* Update shell titles
* duplicate template before modifying it
* update shell title in image
* Add note that not all releases have all common_interfaces
* Don't remove rclpy reference completely
* Update readme for xenial+kinetic
* update ament_index_python API
* Revert "Add note to README about not using fastrtps"
  This reverts commit 52e8c2d5510c85392520b98c23354af40ffd3325.
* fix link order
* update schema url
* add schema to manifest files
* different languages, different comments
* update indentation in templates
* change .template into .em
* Add note to README about not using fastrtps
  * Add note to README about not using fastrtps
* workaround for Python search order
* Add a note about not sourcing multiple workspaces unless instructed
* add note about required ROS 1 version
* update from source build instructions
* add missing install of library
* create library of generated factories
* suppress warning for ROS 1 headers
* use new approach to generate rmw implementation specific targets
* compile generated factories separately from executables
* fix build of bridge for namespace change
* Fix cpplint warning
* ignore unused-parameter warning in ROS 1 message headers
* update docs to use ros1_bridge_listener
* fix qos settings after semantic of rmw_qos_profile_default has changed
* merged some old information back in
* avoid compiler warning in no mappings are available
* fix path for linux
* Account for Linux vs. OSX sed syntax
* Update README.md
* Update README.md
* Update README.md
* Copy bridge instructions from OSX installation doc
* Throw exception
* Update create_subscription
* Use base PublisherBase class
* update code to pass ament_cpplint
* use sensor profile since messages might be large which is not implemented in all rmw impl for reliable qos
* support custom mapping rules
* Update README.md
* Update README.md
* Update README.md
* Update README.md
* add todo
* until we support std/boost::bind use a lambda
* git ignore __pycache\_\_
* remove references on smart pointers
* update link
* update readme
* hide introspection information of internal DDS topics
* only show topic introspection info when passing --show-introspection
* always call ament_package(), even when skipping build
* fail gracefully if pkg-config is not found
* make package only built anything when ROS 1 is available
* use add_executable_for_each_rmw_implementations() from rmw_implementation
* fix mapping rules after renaming ros 2 interface packages
* rename message packages
* use expand_template() from rosidl_cmake
* update to latest changes in rclcpp API
* update dynamic bridge to create unidirection bridges based on runtime topic information
* use pkg-config to find ROS 1 packages
* add another hardcoded topic for ros 2
* catch additional errors when building on OS X
* add explicit build type
* allow the bridge to find Python 2 packages from ROS 1
* raise warning level
* use blocking spin_once
* update automatic mapping rule to allow removing message fields in one ROS version (e.g. Header.seq)
* add hardcoded ROS 2 image topic
* add dynamic version of bridge which looks at ROS 1 topics at runtime, ROS 2 is using a static list
* generate template specialization for all available message types
* add static version of bidirectional bridge for topics base on topic and type string
* renaming
* add simple version of bidirectional bridge for a single specific topic
* add simple version of unidirectional bridge for a single specific topic
* add LICENCE and CONTRIBUTING.md files
* Contributors: Alberto Soragna, ArkadiuszNiemiec, Brian Gerkey, Chris Lalancette, Dirk Thomas, Esteve Fernandez, Hunter Allen, Jackie Kay, Karsten Knese, Mikael Arguedas, Morgan Quigley, Paul Bovbel, Rafal Kozik, Rafał Kozik, Samuel Servulo, Steven! Ragnarök, Tully Foote, William Woodall, dhood, gerkey, locus-services
