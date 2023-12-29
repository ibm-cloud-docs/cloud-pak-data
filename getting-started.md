---

copyright:
  years: 2019, 2023
lastupdated: "2023-12-04"

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
{: shortdesc}

See the [{{site.data.keyword.cpd_full}} readme file](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global/readme/roks/cloud-pak/a5963830-7b4c-4b84-9306-46bf83517d33-global) for detailed information about getting started with {{site.data.keyword.cpd_short}} on IBM Cloud.

Learn more about {{site.data.keyword.cpd_full}} by reviewing the [product documentation](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/overview/overview.html). 

## What's inside this Cloud Pak
{: #whats-in-cloud-pak-for-data}

You can choose which services to install when you install {{site.data.keyword.cpd_full}}. For a complete list, see [Installing services](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-install-services).

## Supported versions
{: #supported-versions}

The current release of {{site.data.keyword.cpd_full_notm}} on IBM Cloud is {{site.data.keyword.cpd_full_notm}} Version 4.7.x.

## Before you begin
{: #prereqs}

Before you can install {{site.data.keyword.cpd_full_notm}}, you must purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html) or register for a 60-day trial license. See [Step 1. Assign the license](#assign_license).

You can deploy Cloud Pak for Data on Virtual Private Cloud (VPC) Gen2 infrastructure. You can use either a single or multi zone deployment. For more information, see [Getting started with Red Hat OpenShift on IBM Cloud](https://cloud.ibm.com/docs/openshift?topic=openshift-getting-started).

You must ensure that you have sufficient resources for the services that you plan to install. For more information, see the [prerequisites](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global#about) for {{site.data.keyword.cpd_full_notm}}.{: note}

### Roles
{: #roles}

To install {{site.data.keyword.cpd_full}} on IBM Cloud, a user must have the following IBM Cloud Identity and Access Management (IAM) roles:

| Role                 | Location                                              | Action           |
|:-------------------- |:------------------------------------------------------|:-----------------|
| Platform Editor      | Manage > Account > Licenses and entitlements          | Assign a license. |
| Service Manager      | Manage > Access (IAM) > Roles > Kubernetes Service             | Run the preinstallation script. |
| Service Writer       | Manage > Access (IAM) > Roles > Kubernetes Service             | Run the installation script. |
| Service Manager in any resource group| Schematics > Workspaces               | Create a workspace. |
| Classic Infrastructure > Services > Storage Manage , Classic Infrastructure > Account > Add/Upgrade Storage   | Manage > Access (IAM) > Users       | Modify the image registry volume. |
{: caption="Table 1. IBM Cloud Identity and Access Management roles required for Cloud Pak for Data" caption-side="bottom"}

For more information, see [Controlling user access with IBM Cloud IAM and Kubernetes RBAC](https://cloud.ibm.com/docs/openshift?topic=openshift-users).

### Storage
{: #storage}

You must ensure that your cluster has sufficient resources and is configured to use supported storage. You can choose one of the following storage options:

- Single zone VPC Gen2 cluster with storage OpenShift® Data Foundation
- Multi zone VPC Gen2 cluster with storage OpenShift® Data Foundation

You must also ensure that your cluster has sufficient resources and is configured to use supported storage.

## Step 1. Assign the license
{: #assign_license}

If you don't already have a license, you can:
* Purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html).
* [Register](https://www.ibm.com/account/reg/us-en/signup?formid=urx-42212) for a 60-day trial license of IBM Cloud Pak for Data.

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
- EnduranceFileStorage - This option uses the storage class `ibmc-file-gold-gid` to install Cloud Pak for Data. For more information, see [Ordering File Storage for Classic](https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-orderingFileStorage). You can use the same storage class while provisioning the instances of services.
- PerformanceFileStorage - This option uses the storage class `ibmc-file-custom-gold-gid` to install Cloud Pak for Data. For more information, see [Ordering File Storage for Classic](https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-orderingFileStorage). You can use the same storage class while provisioning the instances of services.
- Portworx - This option uses the storage class mentioned in [Storage considerations](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/plan/storage_considerations.html). You can use the storage class mentioned in the service instance creation documentation when you provision instances of services.

Specify which services to install when you install {{site.data.keyword.cpd_full_notm}}. For example, to install Watson OpenScale, set `aiopenscale` to `true`.


If you don't select any services to install in this step, only the {{site.data.keyword.cpd_full_notm}} control plane will be installed.

If you want to install a service later, you can return to the **Deployment values** section and set the appropriate parameter to **true** or you can select a service from the {{site.data.keyword.cpd_full_notm}} Services catalog and follow the installation instructions for the service.

For more information, see [Installing IBM Cloud Pak for Data](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/install/install.html).

## Step 6. Install {{site.data.keyword.cpd_full_notm}}
{: #install-cloud-pak-for-data}

1. Ensure that you have assigned a license for {{site.data.keyword.cpd_full_notm}} to the deployment. 
1. Confirm that you have read and agree to the license agreements. 
1. Click **Install**.

The {{site.data.keyword.cpd_full}} automated installation makes the following changes to ensure that services can be installed successfully:
 * Sets kernel parameters. For more information, see [Changing kernel parameter settings](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/install/prep-cluster-node-kernel.html).
 * Enables `noroot squash` on worker nodes for Network File System (NFS). For more information, see [Storage considerations](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/plan/storage_considerations.html).
 
 
## Step 7. Launch your instance of {{site.data.keyword.cpd_full_notm}}
{: #launch-cloud-pak-for-data}

1. After you click **Install**, the **Schematics** > **Workspaces** page opens. You can watch the progress of the installation in the log.
1. When the installation completes, click **Offering dashboard** to access your {{site.data.keyword.cpd_full_notm}} deployment. 
1. Log in to the web client as `admin` using the default password (`password`). Change your password. 
1. On the toolbar, click the **Services** icon and verify that your services are enabled or available.

## Next steps
{: #next-steps}

- To add users to your {{site.data.keyword.cpd_full_notm}} deployment, see [Managing Cloud Pak for Data users](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/admin/users.html).
- To install more services to a deployed cluster, repeat the steps to install from IBM Cloud Catalog and set the required service value to **true** in the **Deployment values** section.
- To install other supported services, such as DataStage, MongoDB, Db2, Db2 Big SQL, Cognos Analytics, Decision Optimization, Db2 Data Gate, Execution Engine for Hadoop, Open Pages or SPSS Modeler, which cannot be automatically installed when you install {{site.data.keyword.cpd_full_notm}} on IBM Cloud, see [Services and integrations](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-nav/head/svc.html).
- To install configure global image pull secrets on your cluster, set the value of configchanges to `Required` and provide your `IBM Cloud API Key` in the apikey, see [Updating the global image pull secret for IBM Cloud Pak for Data](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/install/prep-cluster-global-image-pull-secret.html).
- To uninstall {{site.data.keyword.cpd_full_notm}} or {{site.data.keyword.cpd_full_notm}} services see [Uninstalling](https://cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-uninstalling).
