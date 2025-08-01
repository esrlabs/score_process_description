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

FMEA Fault Models
=================

.. gd_guidl:: FMEA Fault Models
  :id: gd_guidl__fault_models
  :status: valid
  :complies: std_wp__iso26262__software_752, std_req__iso26262__analysis_846

  | Fault Model for sequence diagrams

.. note:: Use the applicable fault models to ensure a structured analysis. If there are additional fault models needed, please enlarge the list of fault models.


.. note:: An ASIL related message is trustable in that manner that it is not corrupted, repeated, lost, delayed, masqueraded or addressed incorrectly.


Fault Models for sequence diagrams
  .. list-table:: Fault Models for sequence diagrams
     :header-rows: 1
     :widths: 15,15,45,15

    * - Element
      - ID
      - Failure Mode
      - Importance (can be used for prioritization)
    * - message
      - MF_01_01
      - message is not received (is a subset/more precise description of MF_01_05)
      - High
    * - message
      - MF_01_02
      - message received too late (only relevant if delay is a realistic fault)
      - Medium
    * - message
      - MF_01_03
      - message received too early (usually not a problem)
      - Low
    * - message
      - MF_01_04
      - message not received correctly by all recipients (different messages or messages partly lost). Only relevant if the same message goes to multiple recipients.
      - High
    * - message
      - MF_01_05
      - message is corrupted
      - High
    * - message
      - MF_01_06
      - message is not sent
      - High
    * - message
      - MF_01_07
      - message is unintended sent
      - High
    * - duration/time constraint
      - CO_01_01
      - minimum constraint boundary is violated
      - Medium
    * - duration/time constraint
      - CO_01_02
      - maximum constraint boundary is violated
      - High
    * - execution
      - EX_01_01
      - Process calculates wrong result(s) (is a subset/more precise description of MF_01_05 or MF_01_04)
      - High
    * - execution
      - EX_01_02
      - processing too slow (only relevant if timing is considered)
      - Medium
    * - execution
      - EX_01_03
      - processing too fast (only relevant if timing is considered)
      - Medium
    * - execution
      - EX_01_04
      - loss of execution
      - High
    * - execution
      - EX_01_05
      - processing changes to arbitrary process
      - Medium
    * - execution
      - EX_01_06
      - processing is not complete (infinite loop)
      - High
