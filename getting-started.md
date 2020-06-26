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

If you want to install a service later, you can return to the **Deployment values** section and set the appropriate parameter to **true** or you can select a service from the Services catalog and follow the installation instructions for the service.

### Apache Spark
{: #apache-spark}

Use the Analytics Engine powered by Apache Spark as a compute engine to run analytical and machine learning jobs. 
- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/spark.html)
- [Installing Apache Spark](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-spark-intro.html)

### Cognos Dashboards
{: #cognos-dashboards}

Use sophisticated visualizations in an analytics project to identify patterns in your data so that you can make timely and effective decisions.
- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/cde.html)
- [Installing Cognos Dashboards](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/cognos/dashboard/dashboard-install.html)

### Data Virtualization
{: #data-virtualization}

Create data sets from disparate data sources so that you can query and use the data as if it came from a single source. 
When you provision this service, check the **My cluster uses Redhat Openshift cluster v3.11** check box. You must check this box if you updated the kernel semaphore parameter check box and you use the `ibmc-file-gold-gid` storage class.

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/dv.html)
- [Installing Data Virtualization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/dv/install-dv.html)

### Db2 Warehouse 
{: #db2-warehouse}
Take advantage of in-memory data processing and in-database analytics in an analytics data warehouse that supports automated scaling.

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/db2wh.html)
- [Installing Db2 Warehouse](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/dbs/db2w-install-ovu.html)


### IBM Streams 
{: #ibm-streams}
Enable continuous and fast analysis of large volumes of moving data so that you can develop and run analytics applications that process in-flight data.

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/streams.html)
- [Installing IBM Streams](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/streams/install-intro.html)

  
### Open Source Management
{: #open-source-management}
Make it easy for developers and data scientists to find and access approved open source packages.

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/osg.html)
- [Installing Open Source Management](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/opensource/opensource-install.html)
  
  
### RStudio Server  
{: #rstudio-server}
Use an integrated development environment for working with R in Watson Studio to create R Shiny applications.

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/rstudio.html)
- [Installing RStudio Server](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/wsj/install-rstudio.html)


### Watson Knowledge Catalog
{: #watson-knowledge-catalog} 

Know your data inside and out. Ensure that your data is high quality, aligns with business objectives, and complies with regulations. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wkc.html)
- [Installing Watson Knowledge Catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-wkc.html)


### Watson Machine Learning
{: #watson-machine-learning}

Build analytical models and neural networks that are trained with your data. Then deploy them into production at scale. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wml.html)
- [Installing Watson Machine Learning](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/wsj/ml-install.html)


### Watson OpenScale
{: #watson-openscale}

Infuse your AI with trust and transparency. Understand how your AI models make decisions to detect and mitigate bias. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/aiopenscale.html)
- [Installing Watson OpenScale](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/openscale/openscale-install-overview.html)


### Watson Studio
{: #watson-studio}

Unearth the meaning in your data. Build custom models and infuse your business with AI and machine learning. 

- [Learn more](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wsl.html)
- [Installing Watson Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-ws.html)


## Supported versions
{: supported-versions}

The current release of {{site.data.keyword.cpd_full_notm}} on IBM Cloud is {{site.data.keyword.cpd_full_notm}} Version 3.0.1.

{{site.data.keyword.cpd_full_notm}} Version 2.1.0.2 on IBM Cloud was deprecated on 25 March 2020. 


## Before you begin
{: #prereqs}

Before you can install {{site.data.keyword.cpd_full_notm}}, you must purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html). 

In addition, you must have a [{{site.data.keyword.openshiftlong_notm}} Version 4.3.18 or above](https://cloud.ibm.com/kubernetes/catalog/openshiftcluster) single-zone cluster on IBM Cloud. Ensure that the cluster has sufficient resources to run {{site.data.keyword.cpd_full_notm}}. For details, see the [prerequisites](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global#about) for {{site.data.keyword.cpd_full_notm}}.

To install Cloud Pak for Data on IBM Cloud, a user must have the following IAM Roles:
 * Account Management > License and Entitlement > Platform Editor role -  To assign a license
 * IAM Services > Schematics > Service Manager role in any resource group -  To create a workspace
 * Classic Infrastructure > Services > Storage Manage , Classic Infrastructure > Account > Add/Upgrade Storage - To modify the image registry volume
 * IAM Services > Kubernetes Service > Service Manager role - To run the pre-install script
 * IAM Services > Kubernetes Service > Service Writer role - To run the install script

IBM Cloud accounts have a default quota of 250 storage volumes. Before you start the installation, ensure that each account has enough storage volumes for Cloud Pak for Data to be installed.
For more information, see [How many volumes can be ordered?](https://cloud.ibm.com/docs/infrastructure/BlockStorage?topic=BlockStorage-block-storage-faqs#how-many-volumes-can-be-ordered).


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
- Creates the security context constraints that are required for Cloud Pak for Data.
- Grants access to the security context constraints to the service accounts that are required for Cloud Pak for Data.



Confirm that the script completes successfully before you proceed.  


## Step 4. Set the deployment values
{: #set-deploy-values}

Use the deployment parameters to specify which services are installed when you install {{site.data.keyword.cpd_full_notm}}:

- To install Apache Spark, set `spark` to `true`.
- To install Cognos Dashboards, set `cde` to `true`.
- To install Data Virtualization, set `dv` to `true`.
- To install Db2 Warehouse, set `db2wh` to `true`.
- To install IBM Streams, set `streams` to `true`.
- To install Open Source Management, set `osg` to `true`.
- To install RStudio Server, set `rstudio` to `true`.
- To install Watson Knowledge Catalog, set `wkc` to `true`.
- To install Watson OpenScale, set `aiopenscale` to `true`.
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
