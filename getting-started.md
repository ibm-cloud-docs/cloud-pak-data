---

copyright:
  years: 2019, 2020
lastupdated: "2020-08-05"

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

You can choose which services to install when you install {{site.data.keyword.cpd_full}}. 

- [Apache Spark](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/spark.html): Use the Analytics Engine powered by Apache Spark as a compute engine to run analytical and machine learning jobs. See [Installing Apache Spark](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-spark-intro.html).

- [Cognos Dashboards](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/cde.html): Use sophisticated visualizations in an analytics project to identify patterns in your data so that you can make timely and effective decisions. See [Installing Cognos Dashboards](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/cognos/dashboard/dashboard-install.html).

- [Data Virtualization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/dv.html): Create data sets from disparate data sources so that you can query and use the data as if it came from a single source. When you provision this service, check the **You must check this box if you updated the kernel semaphore parameter** check box and use the `ibmc-file-gold-gid` storage class. See [Installing Data Virtualization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/dv/install-dv.html).

- [Db2 Warehouse](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/db2wh.html): 
Take advantage of in-memory data processing and in-database analytics in an analytics data warehouse that supports automated scaling. See [Installing Db2 Warehouse](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/dbs/db2w-install-ovu.html).

- [IBM Streams](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/streams.html): 
Enable continuous and fast analysis of large volumes of moving data so that you can develop and run analytics applications that process in-flight data. See [Installing IBM Streams](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/streams/install-intro.html).

- [Open Source Management](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/osg.html)
Make it easy for developers and data scientists to find and access approved open source packages. See [Installing Open Source Management](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/opensource/opensource-install.html).
  
- [RStudio Server](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/rstudio.html) 
Use an integrated development environment for working with R in Watson Studio to create R Shiny applications. See [Installing RStudio Server](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/wsj/install-rstudio.html).

- [Watson Knowledge Catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wkc.html): Know your data inside and out. Ensure that your data is high quality, aligns with business objectives, and complies with regulations. See [Installing Watson Knowledge Catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-wkc.html).

- [Watson Machine Learning](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wml.html): Build analytical models and neural networks that are trained with your data. Then, deploy them into production at scale. See [Installing Watson Machine Learning](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/wsj/ml-install.html).

- [Watson OpenScale](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/aiopenscale.html): Infuse your AI with trust and transparency. Understand how your AI models make decisions to detect and mitigate bias. See [Installing Watson OpenScale](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/openscale/openscale-install-overview.html).

- [Watson Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wsl.html): Build custom models and infuse your business with AI and machine learning. See [Installing Watson Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/wsj/install/install-ws.html).

## Supported versions
{: supported-versions}

The current release of {{site.data.keyword.cpd_full_notm}} on IBM Cloud is {{site.data.keyword.cpd_full_notm}} Version 3.0.1.

## Before you begin
{: #prereqs}

Before you can install {{site.data.keyword.cpd_full_notm}}, you must purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html). See [Step 1. Assign the license](#assign_license).

You also need to configure a [{{site.data.keyword.openshiftlong_notm}} Version 4.3.18 or above](https://cloud.ibm.com/kubernetes/catalog/openshiftcluster) single-zone cluster on IBM Cloud. The minimum requirement for your cluster is 16 cores, 64GB RAM, 1 TB persistent storage per node. For more information, see [Creating a classic OpenShift cluster](https://cloud.ibm.com/docs/openshift?topic=openshift-getting-started#clusters_gs).

This minimum requirement is not sufficient to install all available services on {{site.data.keyword.cpd_full_notm}}. You must ensure that you have sufficient resources for the services that you planned to install. For more information, see the [prerequisites](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global#about) for {{site.data.keyword.cpd_full_notm}}.{:note}

To install {{site.data.keyword.cpd_full}} on IBM Cloud, a user must have the following IBM Cloud Identity and Access Management  (IAM) roles:

| Role                 | Location                                              | Action           |
|:-------------------- |:------------------------------------------------------|:-----------------|
| Platform Editor      | Manage > Account > Licenses and entitlements          | Assign a license |
| Service Manager in any resource group| Schematics                            | Create a workspace |
| Service Manager      | IAM Services > Kubernetes Service                     | Run the pre-install script |
| Service Writer       | IAM Services > Kubernetes Service                     | Run the install script |
| Operator or higher   | Classic Infrastructure > Storage > File Storage<br/>Classic Infrastructure > Account > Add/Upgrade Storage  | Modify the image registry volume |

For more information, see [Setting up access to your cluster](https://cloud.ibm.com/docs/openshift?topic=openshift-users).

IBM Cloud accounts have a default quota of 250 storage volumes. Before you start the installation, ensure that each account has enough storage volumes for {{site.data.keyword.cpd_full}} to be installed. For more information, see [How many volumes can be ordered?](https://cloud.ibm.com/docs/infrastructure/BlockStorage?topic=BlockStorage-block-storage-faqs#how-many-volumes-can-be-ordered)

The {{site.data.keyword.cpd_full}} automated installation makes the following changes to ensure that services can be installed successfully:
 *  Sets kernel parameters.
 *  Enables `noroot squash` on worker nodes for NFS.
 *  Increases the image registry storage size to hold the docker images.

## Step 1. Assign the license
{: #assign_license}

If you don't already have a license, you can:
* Purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html)
* [Register](https://www.ibm.com/account/reg/us-en/signup?formid=urx-42212) for a 60-day trial license of IBM Cloud Pak for Data

**Important**: The trial is for {{site.data.keyword.cpd_full_notm}} software only. The trial does not include entitlement to the Red Hat OpenShift Container Platform.

To assign your license, follow these steps: 
1. Log in to your [IBM Cloud account](https://cloud.ibm.com).
1. On the toolbar, navigate to **Manage** > **Account** and then click **Licenses and entitlements** in the navigation menu.
1. If you don't see any licenses to assign, click **Check IBM Passport Advantage**.
1. Select the appropriate license and click **Assign**.

## Step 2. Configure your installation environment
{: #config-install-env}

Specify where you want to install {{site.data.keyword.cpd_full_notm}}:
1. Select the {{site.data.keyword.openshiftlong_notm}} cluster where you want to deploy {{site.data.keyword.cpd_full_notm}}. 
1. Enter or select the {{site.data.keyword.openshiftlong_notm}} project where you want to deploy {{site.data.keyword.cpd_full_notm}}. 


## Step 3. Configure your workspace
{: #config-workspace}

Specify how you will track and manage your installation from your IBM Cloud Schematics workspace:
1. Enter or select a name for the installation.
1. Consider changing the default resource group. 
1. Specify any tags that you want to use for the installation. Specify multiple tags as a comma-separated list. 


## Step 4. Complete the preinstallation task
{: #pre-install-set-up}

A {{site.data.keyword.openshiftlong_notm}} cluster administrator must complete this step.  Specifically, the administrator must have an [access](https://cloud.ibm.com/docs/openshift?topic=openshift-users) policy in IBM Cloud Identity and Access Management that has an Operator role or higher. 

- If you are not an administrator, use the **Share** link to share the script with your cluster administrator. 
- If you are a cluster administrator, click **Run script** to run the preinstallation set up on your cluster. 

The preinstallation script makes the following changes to your {{site.data.keyword.openshiftlong_notm}} cluster:

- Increases the size of the Docker registry to 200 GB. This change increases the cost of your {{site.data.keyword.openshiftlong_notm}} cluster.
- Creates the security context constraints that are required for {{site.data.keyword.cpd_full}}.
- Grants access to the security context constraints to the service accounts that are required for {{site.data.keyword.cpd_full}}.

Confirm that the script completes successfully before you proceed.  

If the cluster administrator is not allowed to modify the storage, or the infrastructure account is not the same as the current account, a storage administrator can manually execute the script that is provided in [Complete the preinstallation section](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global).

## Step 5. Set the deployment values
{: #set-deploy-values}

Choose a storage class:
- If you want to retain your storage volume, choose the `ibmc-file-retain-gold-gid` storage class.
- Otherwise, choose the `ibmc-file-gold-gid` storage class.

Specify which services to install when you install {{site.data.keyword.cpd_full_notm}}:

- To install Watson OpenScale, set `aiopenscale` to `true`.
- To install Cognos Dashboards, set `cde` to `true`.
- To install Db2 Warehouse, set `db2wh` to `true`.
- To install Data Virtualization, set `dv` to `true`.
- To install Open Source Management, set `osg` to `true`.
- To install RStudio Server, set `rstudio` to `true`.
- To install Apache Spark, set `spark` to `true`.
- To install IBM Streams, set `streams` to `true`.
- To install Watson Knowledge Catalog, set `wkc` to `true`.
- To install Watson Machine Learning, set `wml` to `true`.
- To install Watson Studio, set `wsl` to `true`.

For more information, see  [Installing services](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-install-services).

If you want to install a service later, you can return to the **Deployment values** section and set the appropriate parameter to **true** or you can select a service from the Services catalog and follow the installation instructions for the service.{:tip}

## Step 6. Install {{site.data.keyword.cpd_full_notm}}
{: #install-cloud-pak-for-data}

1. Ensure that you have assigned a license for {{site.data.keyword.cpd_full_notm}} to the deployment. 
1. Confirm that you have read and agree to the license agreements. 
1. Click **Install**.

## Step 7. Launch your instance of {{site.data.keyword.cpd_full_notm}}
{: #launch-cloud-pak-for-data]

1. When the installation completes, click **Offering dashboard** to access your {{site.data.keyword.cpd_full_notm}} deployment or navigate the the **Resources** tab to find your deployment URL. 
1. Log in to the web client as `admin` using the default password (`password`). Change your password. 
1. On the toolbar, click the **Services** icon and verify that your services are enabled or available.

## Next steps
{: #next-steps}

- To add users to your {{site.data.keyword.cpd_full_notm}} deployment, see [Managing users](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/admin/users.html).
- If you want to install more services to a deployed namespace in your cluster, repeat the steps to install from IBM Cloud Catalog and set the required service value to **true** in the **Deployment values** section.
- If you want to install other supported services, such as DataStage, MongoDB, Db2 Advanced Edition, Db2 Big SQL, Cognos Analytics, or Watson Studio Premium, which are not available in the IBM Cloud Catalog, see [Services and integrations](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/svc.html).
- To uninstall {{site.data.keyword.cpd_full_notm}} or {{site.data.keyword.cpd_full_notm}} services see [Uninstalling](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-uninstall).
