---

copyright:
  years: 2019, [{CURRENT_YEAR}]
lastupdated: "[{LAST_UPDATED_DATE}]"

keywords: "uninstalling, getting started, {{site.data.keyword.cpd_short}}, {{ site.data.keyword.datalong }}, data, ai, analytics, data analytics, governance, data governance"

subcollection: cloud-pak-data

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}

# Uninstalling
{: #uninstalling}

You can uninstall services from {{site.data.keyword.data}}, or you can uninstall {{site.data.keyword.data}}.

## Uninstalling {{site.data.keyword.data}}
{: #uninstall_steps}

To uninstall {{site.data.keyword.data}}, you can use the Schematics Workspaces console or the command-line interface.

**Note**: The uninstall action deletes the project. Before you delete a project, make sure that the project does not contain any other applications. For more information, see [Uninstalling the platform and services](https://www.ibm.com/docs/SSNFH6_5.1.x/hub/install/uninstall-platform.html).

To uninstall {{site.data.keyword.data}} from the Schematics Workspaces console, follow these steps:
1. Navigate to **Schematics** > **Workspaces**.
1. Select the workspace of your installed {{site.data.keyword.data}}, and then click **Delete**.
1. Or, click the actions menu for your workspace, and then click **Delete**.
1. Choose **Delete workspace** or **Delete all associated resources** or both, and enter the name of the workspace to confirm.
1. Click **Delete** to delete the workspace and wait for the uninstall to complete.
1. Verify that {{site.data.keyword.data}} is uninstalled by accessing the IBM Managed Red Hat OpenShift Cluster web console and verifying that the components that are related to {{site.data.keyword.data}}, such as any related pods, are no longer installed.

To uninstall {{site.data.keyword.data}} by using the command-line interface, see [Uninstalling an instance of IBM Software Hub](https://www.ibm.com/docs/SSNFH6_5.1.x/hub/install/uninstall-platform-components.html).

## Uninstalling services in {{site.data.keyword.data}}
{: #uninstall_svcs}

To uninstall a service in {{site.data.keyword.data}}, see the uninstall topic for [Services](https://www.ibm.com/docs/SSNFH6_5.1.x/svc-nav/head/services.html).
