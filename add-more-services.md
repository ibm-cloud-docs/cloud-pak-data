---

copyright:
  years: 2019, 2020
lastupdated: "2020-02-20"

keywords: "adding services, getting started, {{site.data.keyword.cpd_short}}, {{site.data.keyword.cpd_full_notm}}, data, ai, analytics, data analytics, governance, data governance"

subcollection: cloud-pak-data

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}


# Adding more services
{: #add-more}


{{site.data.keyword.cpd_short}} includes a subset of services from the IBM cloud catalog.

**Tip**: If you want to install services to your cluster after you install to the existing deployed namespace, repeat the same steps to install from IBM cloud catalog and set the required service value to true in the Deployment values section. You can't install services from the IBM Cloud Schematics workspace by modifying the plan. 

Other supported services on the IBM Managed OpenShift Cluster are: 
- DataStage
- MongoDB
- Db2 Advanced Edition
- Db2 Big SQL
- Cognos Analytics
- Watson Studio Premium

If you want to install these addons, which are not supported by the IBM Cloud Catalog, they must be added manually.
