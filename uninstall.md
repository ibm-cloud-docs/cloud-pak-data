---

copyright:
  years: 2019, 2020
lastupdated: "2020-02-20"

keywords: "getting started tutorial, getting started, {{site.data.keyword.cpd_short}}, {{site.data.keyword.cpd_full_notm}}, data, ai, analytics, data analytics, governance, data governance"

subcollection: cloud-pak-data

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}

# Uninstalling {{site.data.keyword.cpd_full}}

To uninstall {{site.data.keyword.cpd_full}} from the Cloud Catalog, you can use the schematics workspace console or the command line interface.
### Uninstalling {{site.data.keyword.cpd_full}} from the Schematics workspace console
1. Enter the workspace of your installed {{site.data.keyword.cpd_full}}.
2. Click **Actions**, and then click **Delete**.
3. Choose **Delete workspace** and **Delete all associated resources** and enter the name of the workspace to confirm.
4. Click **Delete** to delete the workspace and wait for the uninstall to complete.
5. Verify that {{site.data.keyword.cpd_full}} is uninstalled by accessing the IBM Managed Red Hat OpenShift Cluster web console and verifying that the components that are related to {{site.data.keyword.cpd_full}}, such as any related pods, are no longer installed.

### Uninstalling a service with the command-line
To uninstall {{site.data.keyword.cpd_full}}, see [Uninstalling Cloud Pak for Data](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/install/rhos-uninstall.html).
To uninstall a service in {{site.data.keyword.cpd_full}}, see the uninstall topic for [Services in the catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/services.html).
