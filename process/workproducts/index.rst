..
   # *******************************************************************************
   # Copyright (c) 2025 Contributors to the Eclipse Foundation
   #
   # See the NOTICE file(s) distributed with this work for additional
   # information regarding copyright ownership.
   #
   # This program and the accompanying materials are made available under the
   # terms of the Apache License Version 2.0 which is available at
   # https://www.apache.org/licenses/LICENSE-2.0
   #
   # SPDX-License-Identifier: Apache-2.0
   # *******************************************************************************

Workproducts
============


.. figure:: _assets/wp_traceability_model.drawio.svg
  :width: 100%
  :align: center
  :alt: Project work product traceability model
  :name: wp_traceability_model

  Project development work product traceability model


Platform management
--------------------

General
^^^^^^^

.. workproduct:: Policies
   :id: wp__policies
   :status: draft
   :tags: requirements_management
   :complies: std_wp__iso26262__management_551

   Policies for functional safety and cybersecurity.

.. workproduct:: Training path
   :id: wp__training_path
   :status: draft
   :tags: safety
   :complies: std_wp__iso26262__management_552

   Trainings for safety and security for S-CORE

Process
^^^^^^^

.. workproduct:: Process Definition
   :id: wp__process_definition
   :status: draft
   :tags: process

   Process definitions.

.. workproduct:: Process Management Strategy
   :id: wp__process_plan
   :status: draft
   :tags: process

   Plan to manage and guide execution of the process management activities.


Product development
-------------------

Platform development
^^^^^^^^^^^^^^^^^^^^

.. workproduct:: Platform Build Configuration
   :id: wp__platform_sw_build_config
   :status: draft
   :tags: safety
   :complies: std_wp__iso26262__software_1052

   Build configuration capable to create the SEooC Library for the reference HW, platform level.
   Note: Embedded software in the sense of the Iso (i.e. deployed on the production HW) is not part of our delivery.


Component development
^^^^^^^^^^^^^^^^^^^^^

.. workproduct:: Module Build Configuration
   :id: wp__module_sw_build_config
   :status: draft
   :tags: safety
   :complies: std_wp__iso26262__software_1052

   Build configuration capable to create the SEooC Library for the reference HW, module level.
   Note: Embedded software in the sense of the Iso (i.e. deployed on the production HW) is not part of our delivery.


Supporting activities
---------------------



S-CORE Work product Linkage
---------------------------

.. needpie:: S-CORE workproducts contained in exactly one S-CORE workflow
   :labels: Not-Linked, Linked Workproduct, Linked Workproduct To Multiple Workflows
   :legend:
   :colors: red, green, blue
   :filter-func: score_metamodel.checks.standards.my_pie_workproducts_contained_in_exactly_one_workflow

S-CORE Work product list
------------------------

.. needtable::
   :style: table
   :columns: title;id;tags
   :colwidths: 25,25,25
   :sort: title

   results = []

   for need in needs.filter_types(["workproduct"]):
      if need['is_external'] == False:
                results.append(need)
