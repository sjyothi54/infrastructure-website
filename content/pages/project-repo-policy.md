Title: Project Code Repository Policy

Each Apache project can have a directory in the Apache Subversion repository, or Git repositories, for their product code and assets. The majority of projects now use Git.

  - Each project can have a public directory in the Subversion repository, or as many public Git repositories as their work requires.
  - Each project can also request (using a Jira ticket) that Infra set up **one private Git repository** for use with tasks, such as fixing security issues in project code, that should not be publicly available. The PMC must explain its need of a private repo in the Jira ticket. Only members of the project's PMC can see this repository or read its contents.
    - Private repos **must** have commit/PR/issues emails sent to the project's `private@` list.  

### Git repositories

  1. We recommend using <a href="https://github.com/apache/" target="_blank">GitHub</a> for your interactions with <a href="http://github.com/apache/" target="_blank">writable Git repositories</a>.
  1. Those who have reservations about GitHub's terms and conditions can use Apache's <a href="https://gitbox.apache.org/" target="_blank">GitBox</a>, which also gives full access to Apache's writable Git repositories.
  1. To link your GitHub and Apache IDs, follow <a href="https://gitbox.apache.org/setup/" target="_blank">these instructions</a>.
  1. Projects can request new, blank, public repositories through <a href="https://selfserve.apache.org" target="_blank">selfserve</a>.
  1. Apache does not support custom commits or other hooks. All projects get the same hooks. Setting up <a href="https://github.com/apache/infrastructure-puppet/tree/deployment/modules/gitpubsub" target="_blank">gitpubsub</a> should provide sufficient flexibility without impacting the core Git setup. 

### Subversion directories

Typically, the Incubator PMC makes a Jira request to Infra to create an SVN directory for a graduating project, or for a project joining the ASF with an existing SVN directory. If a project needs a subdirectory for a specific purpose, it requests its creation in a Jira ticket to Infra.

You can find a list of ASF Subversion directories at <a href="https://svn.apache.org/viewvc" target="_blank">svn.apache.org/viewvc</a>.

### Repository access

  1. ASF projects **must** house their project code in ASF supported services (Subversion, GitBox).
  1. Only people with an ICLA on file with Apache can create, edit, or update code housed within the ASF. There is no third-party access to create, edit, or delete files.
  1. Apache software projects are open-source, so everyone has **read** access to all public code housed within the ASF.
  1. Documentation is not code. Projects can host their documentation anywhere (such as on platforms like readthedocs and gitlab) and, if they choose, make them available to the world to create and edit pages.
  1. However, if projects create and house their documentation inside the ASF, statement 2 applies to it.

Since the primary presence of an Apache project must be within Apache, there is an argument for storing project documentation in its own repository alongside the project's code repository. This practice also makes it easier for project committers to move from committing new features, or updates to existing features, to writing about them for the project's users.
