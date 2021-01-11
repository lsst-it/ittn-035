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

   Atlassian is discontinuing on-premise server sales 2Feb2021 and ending support 2Feb2024. RubinObs uses Crowd, Confluence, and Jira, all of which are affected. The Data Center version, which we don't use, will continue.


   
   
.. Do not include the document title (it's automatically added from metadata.yaml).
Questions for Discussion
========================
   1. Should Vera C. Rubin Observatory migrate from on-premise Jira to cloud Jira?
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
- Existing Jira per Project Specific Workflows
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
- Procedures to be used when the Summit or Base are disconnected from the Internet should already been in place

Apps
----
Stakeholders will need to audit their projects for apps (aka add-ons or plugins) currently in use that will not exist in the cloud version.
Solutions or mitigation may be required.

Meta-Data
---------
Some stakeholders may have data within the Jira database related to apps that have been disabled or removed. 
Does the data need to be transferred?
Can it be transferred?

Existing Jira per Project Specific Workflows
--------------------------------------------
Stakeholders will need to review specific workflows to ensure those workflows will operate correctly in a cloud instance.
Stakeholders who access projects directly from MySQL queries need to have updated information to continue with the method, if it is possible.

Altering or Creating Projects, Dashboards, Data fields, Permissions
-------------------------------------------------------------------
Desired configuration may not migrate requiring additional work to recreate various customizations

User Directory Services available with cloud version
-----------------------------------------------------
Our current Jira configuration interacts with Crowd, which interacts with MS Active Directory (AD-LSST) aka LSST Creds or LDAP Account.
Will we continue with this configuration and what of NOIR or other directory services?

License Model and Estimated Upfront and Recurring Costs
-------------------------------------------------------
Wil O'Mullane will check with Atlassian for "free" version. 
Costs should be considered to prepare for any changes in the fee structures. Such changes have occurred with other vendors.

Migration to Cloud
------------------
The production Jira version satisfies the requirement to migrate. However, there are other clean up tasks outlined in the Jira Links.
There are various outlined paths from Move it All to One Project at a Time.
Will URLs be different?
What applications are affected by an URLchanges, i.e. LS.ST

Migration or Integration with NOIR
----------------------------------
NOIR has an existing instance of Jira (need to confirm). 
What considerations should be made to prepare for a migration to or integration with NOIR's instance?

Those Involved
---------------
Declare representatives from the groups of stakeholders and those directly involved in the reviewing, testing and actual work for a successful migration.

Organization and Project Management
-----------------------------------
Is there a desire by Management of either Construction or Operations to implement any changes?

Communicating Reason and Process to Migrate to Set Stakeholder Expectations
---------------------------------------------------------------------------
Communication channels need to be created and managed for the work performed and end-users of the new system.
Any required training should have materials prepared and released in advance of the cut-over.

Backup and Recovery related to configuration mistakes or other changes
----------------------------------------------------------------------
While Atlassian is providing a service and is responsible for maintaining our cloud site, accidental changes or a desire to move away from the service need to be considered. 

The domain to register and what additional, yet to be acquired, domains
-----------------------------------------------------------------------
jira.lsstcorp.org is the primary URL. jira.lsst.org is ready to be implemented after Nginx and Jira are altered. 
Will some sort of Rubin URL be used?

.. .. rubric:: References
Links
=================
- https://www.atlassian.com/blog/announcements/journey-to-cloud
- https://www.atlassian.com/migration/faqs#data-center
- https://www.atlassian.com/migration/faqs
- https://www.atlassian.com/migration/cloud
- https://www.atlassian.com/migration/cloud/guide/introduction/overview
- https://www.atlassian.com/migration/cloud/guide/introduction/requirements
- https://www.atlassian.com/migration/cloud/guide/assess/audit-apps
- https://www.atlassian.com/migration/cloud/guide/assess/assemble-team
- https://www.atlassian.com/migration/cloud/guide/plan/migration-strategy-and-method
- https://www.atlassian.com/migration/cloud/guide/prep/team-and-site#clean-up-instance
- https://confluence.atlassian.com/cloud/set-up-an-atlassian-organization-938859734.html
- https://confluence.atlassian.com/cloud/compare-cloud-migration-methods-981151113.html
- https://confluence.atlassian.com/cloud/assessing-and-migrating-apps-with-the-cloud-migration-assistant-1005322396.html
- https://confluence.atlassian.com/cloud/supported-versions-for-the-jira-cloud-migration-assistant-993925219.html
- https://confluence.atlassian.com/cloud/jira-pre-migration-checklist-1005331549.html
- https://www.atlassian.com/software/jira/guides

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
