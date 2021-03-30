---

copyright:
  years: 2019, 2020, 2021
lastupdated: "2020-11-20"

keywords: "troubleshooting, getting started, {{site.data.keyword.cpd_short}}, {{site.data.keyword.cpd_full_notm}}, data, ai, analytics, data analytics, governance, data governance"

subcollection: cloud-pak-data

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}


# Limitations and known issues
{: #limitations}

* The Cloud Pak for Data on IBM Cloud installation from the IBM Cloud catalog is not supported on Red Hat OpenShift Satellite clusters.

* The installation does not verify whether there are enough resources on the cluster to install {{site.data.keyword.cpd_short}}. 
If you are running other applications on your Red Hat OpenShift cluster, make sure that you have enough resources on the cluster before you install {{site.data.keyword.cpd_short}}.

* When you create a service instance, the service instance initially appears as Failed or Red in the {{site.data.keyword.cpd_short}} console until the persistent volume claim is bound to a persistent volume on the cluster.

* If you see the following message in the installation logs, you can ignore it:
"Error verifying current oauth token - Error from server (NotFound) as install is performed as serviceaccount".

* On the Settings page in **Schematics** > **Workspaces**, you cannot change the **Override value** from `false` to `true` to install a  service. For more information, see  [Installing services](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-install-services).

* On the Settings page in **Schematics** > **Workspaces**, you cannot change the **Override value** from `true` to `false` to uninstall a service. For more information, see  [Uninstalling](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-uninstalling).

For general information about troubleshooting , see [Troubleshooting problems in Cloud Pak for Data](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/cpd/troubleshoot/troubleshooting.html).
