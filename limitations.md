---

copyright:
  years: 2019, 2020
lastupdated: "2020-02-20"

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

* The installation does not verify whether there are enough resources on the cluster to install {{site.data.keyword.cpd_short}}. 
If you are running other applications on your Red Hat OpenShift cluster, make sure that you have enough resources on the cluster before you install {{site.data.keyword.cpd_short}}.

* When service instances are created, they initially appear as Failed or Red because the persistent volume claims take some time to bound.

* The installation is not supported on IBM Managed Red Hat OpenShift Cluster VPC (Gen2). It supports the classic infrastructure only.

* In the error log, the error message "Error verifying current oauth token - Error from server (NotFound) as install is performed as serviceaccount" can be ignored.

For general information about troubleshooting , see [Troubleshooting problems in Cloud Pak for Data](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/troubleshoot/troubleshooting.html).
