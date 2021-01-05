..
  Technote content.

  See https://developer.lsst.io/restructuredtext/style.html
  for a guide to reStructuredText writing.

  Do not put the title, authors or other metadata in this document;
  those are automatically added.

  Use the following syntax for sections:

  Sections
  ========

  and

  Subsections
  -----------

  and

  Subsubsections
  ^^^^^^^^^^^^^^

  To add images, add the image file (png, svg or jpeg preferred) to the
  _static/ directory. The reST syntax for adding the image is

  .. figure:: /_static/filename.ext
     :name: fig-label

     Caption text.

   Run: ``make html`` and ``open _build/html/index.html`` to preview your work.
   See the README at https://github.com/lsst-sqre/lsst-technote-bootstrap or
   this repo's README for more info.

   Feel free to delete this instructional comment.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. TODO: Delete the note below before merging new content to the master branch.

.. note::

   **This technote is not yet published.**

   Atlassian is discontinuing on-premise server sales 2Feb2021 and ending support 2Feb2024. RubinObs uses Crowd, Confluence, and Jira, all of which are affected.


   Questions for Discussion
   ========================
   1. Should Vera C. Rubin Observator (RubinObs) migrate from on-premise Jira to cloud Jira?
   2. If Jira is moved to the cloud, should Crowd and Confluence migrate as well?
   3. Who are the group and individual stakeholders?
   
   Current Answers before Discussion
   =================================
   1. To be determined.
   2. Assumed Yes.
   3. Rubin Construction (PMO); Rubin Operations; End Users; Project Owners: DM, SE, IT, TSS, Travel, Publications; NOIR(?);
   
   Discussion Topics
   =================
 - Apps (aka add-ons or plugins) used by stakeholders not suppored in the cloud
 - Meta-Data stored in the database related to disabled, obsolete yet enabled, or removed apps
 - Existing Project Specific Workflows
 - Altering or Creating Projects, Dashboards, Data fields, Permissions
 - User Directory Services available with cloud version
 - License Model and Estimated Upfront and Recurring Costs
 - Migration to Cloud
 - Migration or Integration with NOIR
 - Those Invovled: Stakeholders; more specifically, groups or individual tasked with project or team based assessment and audit of how apps are currently used; tasked with preparing change managent for each project; testing and validating the migration; performing the migration and cut-over
 - Backup and Recovery related to configuration mistakes or other changes
 - The domain to register and what additional, yet to be acquired, domains
 - Organization and Project Management
 - Communicating Reason and Process to Migrate to Set Stakeholder Expectations
   
.. Do not include the document title (it's automatically added from metadata.yaml).

.. .. rubric:: References
 - https://www.atlassian.com/blog/announcements/journey-to-cloud

https://www.atlassian.com/migration/faqs

https://www.atlassian.com/migration/cloud

https://www.atlassian.com/migration/cloud/guide/introduction/overview

https://www.atlassian.com/migration/cloud/guide/introduction/requirements

https://www.atlassian.com/migration/cloud/guide/assess/audit-apps

https://www.atlassian.com/migration/cloud/guide/assess/assemble-team

https://www.atlassian.com/migration/cloud/guide/plan/migration-strategy-and-method

https://www.atlassian.com/migration/cloud/guide/prep/team-and-site#clean-up-instance

https://confluence.atlassian.com/cloud/set-up-an-atlassian-organization-938859734.html

https://confluence.atlassian.com/cloud/compare-cloud-migration-methods-981151113.html

https://confluence.atlassian.com/cloud/assessing-and-migrating-apps-with-the-cloud-migration-assistant-1005322396.html

https://confluence.atlassian.com/cloud/supported-versions-for-the-jira-cloud-migration-assistant-993925219.html

https://confluence.atlassian.com/cloud/jira-pre-migration-checklist-1005331549.html

https://www.atlassian.com/software/jira/guides

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
