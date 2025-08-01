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

.. _feature_template:

[Your Feature Name]
###################

.. note:: Document header

.. document:: [Your Feature Name]
   :id: doc__feature_name
   :status: draft
   :safety: ASIL_B
   :realizes: wp__feat_request
   :tags: template

.. attention::
    The above directive must be updated according to your Feature.

    - Modify ``document`` to be your Feature Name
    - Modify ``id`` to be your Feature Name in upper snake case preceded by ``doc__``
    - Adjust ``status`` to be ``valid``
    - Adjust ``safety`` and ``tags`` according to your needs

Feature flag
============

To activate this feature, use the following feature flag:

``experimental_[your_feature_name]``

    .. note::
     The feature flag must reflect the feature name in snake_case. Further, it is prepended with ``experimental_``, as
     long as the feature is not yet stable.

Abstract
========

[A short (~200 word) description of the contribution being addressed.]


Motivation
==========

[Clearly explain why the existing platform/project solution is inadequate to address the topic that the CR solves.]

    .. note::
     The motivation is critical for CRs that want to change the existing features or infrastructure.
     It should clearly explain why the existing solution is inadequate to address the topic that the CR solves.
     Motivation may based on criteria as resource requirements, scheduling issues, risks, benefits, etc.
     CRs submissions without sufficient motivation may be rejected.



Rationale
=========

[Describe why particular design decisions were made.]


   .. note::
      The rationale should provide evidence of consensus within the community and discuss important objections or concerns raised during discussion.


Specification
=============

[Describe the requirements, architecture of any new feature.] or
[Describe the change to requirements, architecture, implementation, process, documentation, infrastructure of any change request.]

   .. note::
      A CR shall specify the stakeholder requirements as part of our platform/project.
      Thereby the :need:`rl__technical_lead` will approve these requirements as part of accepting the CR (e.g. merging the PR with the CR).



Backwards Compatibility
=======================

[Describe potential impact (especially including safety and security impacts) and severity on pre-existing platform/project elements.]


Security Impact
===============

[How could a malicious user take advantage of this new/modified feature?]

   .. note::
      If there are security concerns in relation to the CR, those concerns should be explicitly written out to make sure reviewers of the CR are aware of them.

Which security requirements are affected or has to be changed?
Could the new/modified feature enable new threat scenarios?
Could the new/modified feature enable new attack paths?
Could the new/modified feature impact functional safety?
If applicable, which additional security measures must be implemented to mitigate the risk?

    .. note::
     Use Trust Boundary, Defense in Depth Analysis and/or Security Software Critically Analysis,
     Vulnerability Analysis.
     [Methods will be defined later in Process area Security Analysis]
     These analyses may not be available at the time of creation of the feature (request) but content will be improved iteratively.

Safety Impact
=============

[How could the safety be impacted by the new/modified feature?]

   .. note::
      If there are safety concerns in relation to the CR, those concerns should be explicitly written out to make sure reviewers of the CR are aware of them.
      Link here to the filled out :need:`Impact Analysis Template <gd_temp__change__impact_analysis>` or copy the template in this chapter.

Which safety requirements are affected or has to be changed?
Could the new/modified feature be a potential common cause or cascading failure initiator?
If applicable, which additional safety measures must be implemented to mitigate the risk?

    .. note::
     Use Dependency Failure Analysis and/or Safety Software Critically Analysis.
     [Methods will be defined later in Process area Safety Analysis]
     These analyses may not be available at the time of creation of the feature (request) but content will be improved iteratively.

For new feature contributions:

[What is the expected ASIL level?]


License Impact
==============

[How could the copyright impacted by the license of the new contribution?]


How to Teach This
=================

[How to teach users, new and experienced, how to apply the CR to their work.]

   .. note::
      For a CR that adds new functionality or changes behavior, it is helpful to include a section on how to teach users, new and experienced, how to apply the CR to their work.



Rejected Ideas
==============

[Why certain ideas that were brought while discussing this CR were not ultimately pursued.]

   .. note::
      Throughout the discussion of a CR, various ideas will be proposed which are not accepted.
      Those rejected ideas should be recorded along with the reasoning as to why they were rejected.
      This both helps record the thought process behind the final version of the CR as well as preventing people from bringing up the same rejected idea again in subsequent discussions.
      In a way this section can be thought of as a breakout section of the Rationale section that is focused specifically on why certain ideas were not ultimately pursued.



Open Issues
===========

[Any points that are still being decided/discussed.]

   .. note::
       While a CR is in draft, ideas can come up which warrant further discussion.
       Those ideas should be recorded so people know that they are being thought about but do not have a concrete resolution.
       This helps make sure all issues required for the CR to be ready for consideration are complete and reduces people duplicating prior discussion.



Footnotes
=========

[A collection of footnotes cited in the CR, and a place to list non-inline hyperlink targets.]


.. toctree::
   :hidden:

   requirements/index.rst
   architecture/index.rst
   safety_planning/index.rst
   safety_analysis/fmea.rst
   safety_analysis/dfa.rst
   safety_analysis/platform_dfa.rst
