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


FMEA (Failure Modes and Effects Analysis)
=========================================

.. document:: [Your Feature Name] FMEA
   :id: doc__feature_name_fmea
   :status: draft
   :safety: ASIL_B
   :realizes: wp__feature_fmea
   :tags: template

.. note:: Use the content of the document to describe e.g. why a fault model is not applicable for the diagram.

.. attention::
    The above directive must be updated according to your Feature.

    - Modify ``Your Feature Name`` to be your Feature Name
    - Modify ``id`` to be your Feature Name in upper snake case preceded by ``doc__`` and succeeded by ``_fmea``
    - Adjust ``status`` to be ``valid``
    - Adjust ``safety`` and ``tags`` according to your needs

Failure Mode List
-----------------

.. code-block:: rst


    .. feat_saf_fmea:: <Title>
       :violates: <Feature architecture>
       :id: feat_saf_fmea__<Feature>__<Element descriptor>
       :fault_id: <ID from fault model :need:`gd_guidl__fault_models`>
       :failure_effect: "description of failure effect of the fault model on the element"
       :mitigated_by: <ID from Feature Requirement | ID from AoU Feature Requirement>
       :mitigation_issue: <ID from Issue Tracker>
       :sufficient: <yes|no>
       :status: <valid|invalid>

 .. note::   argument is inside the 'content'. Therefore content is mandatory

.. attention::
    The above directive must be updated according to your feature FMEA.

    - The above "code-block" directive must be updated
    - Fill in all the needed information in the <brackets>
