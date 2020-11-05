---

copyright:
  years: 2019, 2020
lastupdated: "2020-09-15"

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

- [Apache Spark](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/spark.html): Use the Analytics Engine powered by Apache Spark as a compute engine to run analytical and machine learning jobs.
- [Cognos Dashboards](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/cde.html): Use sophisticated visualizations in an analytics project to identify patterns in your data so that you can make timely and effective decisions.
- [Data Virtualization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/dv.html): Create data sets from disparate data sources so that you can query and use the data as if it came from a single source. When you provision this service, check the **You must check this box if you updated the kernel semaphore parameter** check box and use the `ibmc-file-gold-gid` storage class.
- [Db2 Data Gate](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/dg.html)
Extract, load, and synchronize your mission-critical data from Db2 for z/OS to Cloud Pak for Data for quick access by your new, high volume, read-only transactional, and analytic applications.
- [Db2 Warehouse](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/db2wh.html): 
Take advantage of in-memory data processing and in-database analytics in an analytics data warehouse that supports automated scaling. When Db2 Warehouse is installed, [Db2 Data Management Console](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/dmc.html) is also installed.
- [RStudio Server](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/rstudio.html) 
Use an integrated development environment for working with R in Watson Studio to create R Shiny applications.
- [Streams](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/streams.html): 
Enable continuous and fast analysis of large volumes of moving data so that you can develop and run analytics applications that process in-flight data. When IBM Streams is installed, [Streams Flows](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/stflows.html) is also installed.
- [Watson Knowledge Catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wkc.html): Know your data inside and out. Ensure that your data is high quality, aligns with business objectives, and complies with regulations.
- [Watson Machine Learning](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wml.html): Build analytical models and neural networks that are trained with your data. Then, deploy them into production at scale. 
- [Watson OpenScale](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/aiopenscale.html): Infuse your AI with trust and transparency. Understand how your AI models make decisions to detect and mitigate bias. 
- [Watson Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wsl.html): Build custom models and infuse your business with AI and machine learning.

## Supported versions
{: supported-versions}

The current release of {{site.data.keyword.cpd_full_notm}} on IBM Cloud is {{site.data.keyword.cpd_full_notm}} Version 3.5.0.

## Before you begin
{: #prereqs}

Before you can install {{site.data.keyword.cpd_full_notm}}, you must purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html) or register for a 60-day trial license. See [Step 1. Assign the license](#assign_license).

You also need to configure an [IBM Red Hat OpenShift Version 4.5.4 or above](https://cloud.ibm.com/kubernetes/catalog/openshiftcluster) classic cluster on IBM Cloud. The minimum requirement for your cluster is 16 cores and 64GB RAM per node. For more information, see [Creating a classic OpenShift cluster](https://cloud.ibm.com/docs/openshift?topic=openshift-getting-started#clusters_gs).

This minimum CPU and memory requirement is not sufficient to install all available services on {{site.data.keyword.cpd_full_notm}}. You must ensure that you have sufficient resources for the services that you plan to install. For more information, see the [prerequisites](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global#about) for {{site.data.keyword.cpd_full_notm}}.{:note}

### Roles
To install {{site.data.keyword.cpd_full}} on IBM Cloud, a user must have the following IBM Cloud Identity and Access Management  (IAM) roles:

| Role                 | Location                                              | Action           |
|:-------------------- |:------------------------------------------------------|:-----------------|
| Platform Editor      | Manage > Account > Licenses and entitlements          | Assign a license |
| Service Manager      | Manage > Access (IAM) > Roles > Kubernetes Service             | Run the pre-install script |
| Service Writer       | Manage > Access (IAM) > Roles > Kubernetes Service             | Run the install script |
| Service Manager in any resource group| Schematics > Workspaces               | Create a workspace |
| Classic Infrastructure > Services > Storage Manage , Classic Infrastructure > Account > Add/Upgrade Storage   | Manage > Access (IAM) > Users       | Modify the image registry volume |

For more information, see [Setting up access to your cluster](https://cloud.ibm.com/docs/openshift?topic=openshift-users).

### Storage
You must ensure that your cluster has sufficient resources and is configured to use supported storage. You can choose one of the following storage options:
- Single zone classic cluster with storage IBM Cloud File Storage
- Single zone classic cluster with storage IBM Cloud Portworx Enterprise
- Multi zone classic cluster with storage IBM Cloud Portworx Enterprise

If you are using a single zone classic cluster with IBM Cloud File Storage, IBM Cloud accounts have a default quota of 250 storage volumes. Before you start the installation, ensure that each account has enough storage volumes for {{site.data.keyword.cpd_full}} to be installed. For more information, see [How many volumes can be ordered?](https://cloud.ibm.com/docs/infrastructure/FileStorage?topic=FileStorage-file-storage-faqs#how-many-volumes-can-be-ordered)

If you are using Portworx storage, you must configure IBM Cloud Portworx Enterprise on the cluster before you start the Cloud Pak for Data installation. For more information, see [Configure Portworx](https://cloud.ibm.com/docs/openshift?topic=openshift-portworx). You must use the 10 IOPS/GB option for the Endurance block storage used to configure Portworx.

## Step 1. Assign the license
{: #assign_license}

If you don't already have a license, you can:
* Purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html)
* [Register](https://www.ibm.com/account/reg/us-en/signup?formid=urx-42212) for a 60-day trial license of IBM Cloud Pak for Data

**Important**: The trial is for {{site.data.keyword.cpd_full_notm}} software only. The trial does not include entitlement to the Red Hat OpenShift Container Platform.

To assign your license, follow these steps: 
1. Log in to your [IBM Cloud account](https://cloud.ibm.com).
1. If you don't see any licenses to assign, navigate to **Manage** > **Account** and then click **Licenses and entitlements** in the navigation menu.
1. If there are no licenses to assign on the **Licenses and entitlements** page, click **Check IBM Passport Advantage**.
1. Select the appropriate license and click **Assign**.

## Step 2. Configure your installation environment
{: #config-install-env}

Specify where you want to install {{site.data.keyword.cpd_full_notm}}:
1. Select the {{site.data.keyword.openshiftlong_notm}} cluster where you want to deploy {{site.data.keyword.cpd_full_notm}}. 
1. Enter or select the {{site.data.keyword.openshiftlong_notm}} project where you want to deploy {{site.data.keyword.cpd_full_notm}}. 


## Step 3. Configure your workspace
{: #config-workspace}

Specify how you will track and manage your installation:
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
- EnduranceFileStorage - This option uses the storage class `ibmc-file-gold-gid` to install Cloud Pak for Data. For more information, see [Endurance Storage](https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-about#provisioning-with-endurance-tiers). You can use the same storage class while provisioning the instances of services.
- PerformanceFileStorage - This option uses the storage class `ibmc-file-custom-gold-gid` to install Cloud Pak for Data. For more information, see [Performance Storage](https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-about#provisioning-with-performance). You can use the same storage class while provisioning the instances of services.
- Portworx - This option uses the storage class mentioned in [Storage considerations](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/plan/storage_considerations.html). You can use the storage class mentioned in the service instance creation documentation when you provision instances of services.

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

If you don't select any services to install in this step, only the {{site.data.keyword.cpd_full_notm}} control plane will be installed.

If you want to install a service later, you can return to the **Deployment values** section and set the appropriate parameter to **true** or you can select a service from the {{site.data.keyword.cpd_full_notm}} Services catalog and follow the installation instructions for the service.{:tip}

For more information, see [Installing services](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-install-services).

## Step 6. Install {{site.data.keyword.cpd_full_notm}}
{: #install-cloud-pak-for-data}

1. Ensure that you have assigned a license for {{site.data.keyword.cpd_full_notm}} to the deployment. 
1. Confirm that you have read and agree to the license agreements. 
1. Click **Install**.

The {{site.data.keyword.cpd_full}} automated installation makes the following changes to ensure that services can be installed successfully:
 * Sets kernel parameters. For more information, see [Kernel parameter settings](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/install/node-settings.html#node-settings__kernel#node-settings__kernel).
 * Enables `noroot squash` on worker nodes for Network File System (NFS). For more information, see [Storage considerations](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/plan/storage_considerations.html).
 * Increases the image registry storage size to hold the docker images. For more information, see [Setting up your registry server](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/install/registry_server.html).
 
 
## Step 7. Launch your instance of {{site.data.keyword.cpd_full_notm}}
{: #launch-cloud-pak-for-data}

1. After you click **Install**, the **Schematics** > **Workspaces** page opens. You can watch the progress of the installation in the log.
1. When the installation completes, click **Offering dashboard** to access your {{site.data.keyword.cpd_full_notm}} deployment. 
1. Log in to the web client as `admin` using the default password (`password`). Change your password. 
1. On the toolbar, click the **Services** icon and verify that your services are enabled or available.

## Next steps
{: #next-steps}

- To add users to your {{site.data.keyword.cpd_full_notm}} deployment, see [Managing users](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/admin/users.html).
- To install more services to a deployed cluster, repeat the steps to install from IBM Cloud Catalog and set the required service value to **true** in the **Deployment values** section.
- To install other supported services, such as DataStage, MongoDB, Db2, Db2 Big SQL, Cognos Analytics, Decision Optimization, Db2 Data Gate, Execution Engine for Hadoop, or SPSS Modeler, which cannot be automatically installed when you install {{site.data.keyword.cpd_full_notm}} on IBM Cloud, see [Services and integrations](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/svc.html).
- To uninstall {{site.data.keyword.cpd_full_notm}} or {{site.data.keyword.cpd_full_notm}} services see [Uninstalling](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-uninstalling).
