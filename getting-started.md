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


# Getting started with {{site.data.keyword.cpd_full_notm}}
{: #getting-started}

Collect, organize, and analyze your data to generate meaningful insight with an extensible, end-to-end platform for governance, analytics, and AI that runs on {{site.data.keyword.openshiftlong_notm}}. With {{site.data.keyword.cpd_full}}, it's easy to find and access trusted data so that you can put your data to work quickly and efficiently. Make data-driven decisions and operationalize AI with trust and transparency throughout your business. 
{:shortdesc}

Learn more about {{site.data.keyword.cpd_full}} by reviewing the [product documentation](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/overview/overview.html). 



## What's inside this Cloud Pak
{: #whats-in-cloud-pak-for-data}

The features that you can use depend on the services that you install. You can choose which services to install when you install {{site.data.keyword.cpd_full}}. 

If you want to install a service later, you can follow the documented installation procedure. 


### Data Virtualization
{: #data-virtualization}

Create data sets from disparate data sources so that you can query and use the data as if it came from a single source.

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/dv/dv_overview.html)
- [Installing Data Virtualization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/dv/install-dv.html)


### Watson Knowledge Catalog
{: #watson-knolwedge-catalog} 

Know your data inside and out. Ensure that your data is high quality, aligns with business objectives, and complies with regulations. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/catalog/overview-wkc.html)
- [Installing Watson Knowledge Catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-wkc.html)


### Watson Studio
{: #watson-studio}

Unearth the meaning in your data. Build custom models and infuse your business with AI and machine learning. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/getting-started/overview-ws.html)
- [Installing Watson Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-ws.html)


### Watson Machine Learning
{: #watson-machine-learning}

Build analytical models and neural networks that are trained with your data. Then deploy them into production at scale. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/analyze-data/ml-install-overview.html)
- [Installing Watson Machine Learning](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/wsj/ml-install.html)


### Watson OpenScale
{: #watson-openscale}

Infuse your AI with trust and transparency. Understand how your AI models make decisions to detect and mitigate bias. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/openscale/openscale-overview.html)
- [Installing Watson OpenScale](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/openscale/openscale-install-overview.html)




## Before you begin
{: #prereqs}

Before you can install IBM Cloud Pak for Data, you must purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html). 

In addition, you must have a [{{site.data.keyword.openshiftlong_notm}} Version 3.11 cluster](https://cloud.ibm.com/kubernetes/catalog/openshiftcluster) on IBM Cloud. Ensure that the cluster has sufficient resources to run {{site.data.keyword.cpd_full_notm}}. For details, see the [prerequisites](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global#about) for {{site.data.keyword.cpd_full_notm}}.


## Step 1. Configure your installation environment
{: #config-install-env}

It is recommended that you install only one instance of {{site.data.keyword.cpd_full_notm}} on each {{site.data.keyword.openshiftlong_notm}} cluster. 

Specify where you want to install {{site.data.keyword.cpd_full_notm}}:
1. Select the {{site.data.keyword.openshiftlong_notm}} cluster where you want to deploy {{site.data.keyword.cpd_full_notm}}. 
1. Enter or select the {{site.data.keyword.openshiftlong_notm}} project where you want to deploy {{site.data.keyword.cpd_full_notm}}. 


## Step 2. Configure your workspace
{: #config-workspace}

Specify how you will track and manage your installation from your IBM Cloud Schematics workspace:
1. Enter or select a name for the installation.
1. Specify any tags that you want to use for the installation. Specify multiple tags as a comma-separated list. 


## Step 3. Complete the preinstallation set up
{: #pre-install-set-up}

A {{site.data.keyword.openshiftlong_notm}} cluster administrator must complete this step.  Specifically, the administrator must have an [access](https://cloud.ibm.com/docs/openshift?topic=openshift-users) policy in IBM Cloud Identity and Access Management that has an Operator role or higher. 

- If you are not an administrator, use the **Share** link to share the script with your cluster administrator. 
- If you are a cluster administrator, click **Run script** to run the preinstallation set up on your cluster. 

The preinstallation script makes the following changes to your {{site.data.keyword.openshiftlong_notm}} cluster:

- Increases the size of the Docker registry to 200 GB. 
  This change increases the cost of your {{site.data.keyword.openshiftlong_notm}} cluster.
- Increases IOPS to 10. 
  This change increases the cost of your {{site.data.keyword.openshiftlong_notm}} cluster.
- Creates the security context constraints that are required for Cloud Pak for Data.
- Grants access to the security context constraints to the service accounts that are required for Cloud Pak for Data.



Confirm that the script completes successfully before you proceed.  


## Step 4. Set the deployment values
{: #set-deploy-values}

Use the deployment parameters to specify which services are installed when you install {{site.data.keyword.cpd_full_notm}}:

- To install Watson OpenScale, set `aiopenscale` to `true`.
- To install Data Virtualization, set `dv` to `true`.
- To install Watson Knowledge Catalog, set `wkc` to `true`.
- To install Watson Machine Learning, set `wml` to `true`.
- To install Watson Studio, set `wsl` to `true`.



## Step 5. Install {{site.data.keyword.cpd_full_notm}}
{: #install-cloud-pak-for-data}

1. Ensure that you have assigned a license for {{site.data.keyword.cpd_full_notm}} to the deployment. 
1. Confirm that you have read and agree to the license agreements. 
1. Click **Install**.



## Next steps
{: #next-steps}

When the installation completes, you can access your {{site.data.keyword.cpd_full_notm}} deployment with the provided URL. 

Log in to the web client as `admin` using the default password (`password`). Change your password. 

For details on creating additional users, see [Managing users](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/admin/users.html).
