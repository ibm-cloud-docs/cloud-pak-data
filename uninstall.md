---

copyright:
  years: 2019, [{CURRENT_YEAR}]
lastupdated: "[{LAST_UPDATED_DATE}]"

keywords: "uninstalling, getting started, {{site.data.keyword.cpd_short}}, {{site.data.keyword.cpd_full_notm}}, data, ai, analytics, data analytics, governance, data governance"

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

You can uninstall services from {{site.data.keyword.cpd_full}}, or you can uninstall {{site.data.keyword.cpd_full}}.

## Uninstalling {{site.data.keyword.cpd_full}}
{: #uninstall_steps}

To uninstall {{site.data.keyword.cpd_full}}, you can use the Schematics Workspaces console or the command-line interface.

**Note**: The uninstall action deletes the project. Before you delete a project, make sure that the project does not contain any other applications. For more information, see [Uninstalling the platform and services](https://www.ibm.com/docs/SSQNUZ_5.0.x/cpd/install/uninstall-platform.html).

To uninstall {{site.data.keyword.cpd_full}} from the Schematics Workspaces console, follow these steps:
1. Navigate to **Schematics** > **Workspaces**.
1. Select the workspace of your installed {{site.data.keyword.cpd_full}}, and then click **Delete**.
1. Or, click the actions menu for your workspace, and then click **Delete**.
1. Choose **Delete workspace** or **Delete all associated resources** or both, and enter the name of the workspace to confirm.
1. Click **Delete** to delete the workspace and wait for the uninstall to complete.
1. Verify that {{site.data.keyword.cpd_full}} is uninstalled by accessing the IBM Managed Red Hat OpenShift Cluster web console and verifying that the components that are related to {{site.data.keyword.cpd_full}}, such as any related pods, are no longer installed.

To uninstall {{site.data.keyword.cpd_full}} by using the command-line interface, see [Uninstalling an instance of IBM Cloud Pak for Data](https://www.ibm.com/docs/SSQNUZ_5.0.x/cpd/install/uninstall-platform-components.html).

## Uninstalling services in {{site.data.keyword.cpd_full}}
{: #uninstall_svcs}

To uninstall a service in {{site.data.keyword.cpd_full}}, see the uninstall topic for [Services and integrations](https://www.ibm.com/docs/SSQNUZ_5.0.x/svc-nav/head/services.html).
