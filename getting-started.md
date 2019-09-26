<!-- Name your file `getting-started.md` and include it in the Learn navigation group in your toc file. -->

---

copyright:
  years: 2019
lastupdated: "2019-09-25"

keywords: "getting started tutorial, getting started, {{site.data.keyword.cpd_short}}, {{site.data.keyword.cpd_full_notm}}, data, ai, analytics, data analytics, governance, data governance"

subcollection: cloud-pak-data

---

<!-- Common attributes used in the template are defined as follows: -->
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}


# Getting started with {{site.data.keyword.cpd_full_notm}}
{: #getting-started}

Collect, organize, and analyze your data to generate meaningful insight with an extensible, end-to-end platform for governance, analytics, and AI that runs on Red Hat OpenShift. With {{site.data.keyword.cpd_full}}, it's easy to find and access trusted data so that you can put your data to work quickly and efficiently. Make data-driven decisions and operationalize AI with trust and transparency throughtout your business. 
{:shortdesc}

Learn more about {{site.data.keyword.cpd_full}} by reviewing the [product documentation](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/com.ibm.icpdata.doc/zen/overview/overview.html). 



## What's inside this Cloud Pak
{: #whats-in-cloud-pak-for-data}

{{site.data.keyword.cpd_full_notm}} includes the following services:


### Analytics Dashboards 
{: #analytics-dashboards}

A drag-and-drop canvas that enables you to create interactive data visualizations. Identify patterns in your data with
sophisticated visualizations. No coding needed. For details, see [Analytics dashboards](https://www.ibm.com/support/knowledgecenter/SSQNUZ_2.1.0/com.ibm.icpdata.doc/dashboard/c_parent_topic.html).


### Watson Studio
{: #watson-studio}

A collaborative data science environment with a variety of tools that enable you to shape, cleanse, and analyze data. For details, see [Analyzing data](https://www.ibm.com/support/knowledgecenter/SSQNUZ_2.1.0/com.ibm.icpdata.doc/dsx/analyze-data.html).


### Unified Governance and Integration
{: #unified-governance}

A suite of data governance tools that enable you to curate your data so that it's useful, trusted, and ready to analyze. For details, see the following topics:
- [Cataloging and governing data](https://www.ibm.com/support/knowledgecenter/SSQNUZ_2.1.0/com.ibm.icpdata.doc/igc/catalog-govern-overview.html)
- [Exploring and profiling data](https://www.ibm.com/support/knowledgecenter/SSQNUZ_2.1.0/com.ibm.icpdata.doc/igc/explore-profile-overview.html)
- [Transforming data with ETL](https://www.ibm.com/support/knowledgecenter/SSQNUZ_2.1.0/com.ibm.icpdata.doc/dfd/c_transf_data.html) 


### See the full catalog of offerings
{: #full-catalog}

{{site.data.keyword.cpd_full_notm}} includes a variety of services. See the {{site.data.keyword.cpd_full_notm}} documentation for a [complete list of services](https://www.ibm.com/support/knowledgecenter/SSQNUZ_2.1.0/com.ibm.icpdata.doc/zen/admin/add-ons.html).


## Before you begin
{: #prereqs}

Before you can install IBM Cloud Pak for Data, you must purchase a license through [IBM Passport Advantage](https://www.ibm.com/software/passportadvantage/index.html). 

In addition, you must have a [Red Hat OpenShift cluster](https://cloud.ibm.com/kubernetes/catalog/openshiftcluster) on IBM Cloud. Ensure that the cluster has sufficient resources to run {{site.data.keyword.cpd_full_notm}}. For details, see the [prerequisites](https://cloud.ibm.com/catalog/content/ibm-cp-data#about) for {{site.data.keyword.cpd_full_notm}}.


## Step 1. Configure your installation environment
{: #config-install-env}

It is recommended that you install only one instance of {{site.data.keyword.cpd_full_notm}} on each Red Hat OpenShift cluster. 

Specify where you want to install {{site.data.keyword.cpd_full_notm}}:
1. Select the Red Hat OpenShift cluster where you want to deploy {{site.data.keyword.cpd_full_notm}}. 
1. Enter or select the project where you want to deploy {{site.data.keyword.cpd_full_notm}}. 


## Step 2. Configure your workspace
{: #config-workspace}

Specify how you will track and manage your installation from your IBM Cloud Schematics workspace:
1. Enter or select a name for the installation.
1. Specify any tags that you want to use for the installation. Specify multiple tags as a comma-separated list. 


## Step 3. Complete the pre-installation check
{: #pre-install-check}

A Red Hat OpenShift cluster administrator must complete this step.

- If you are not an administrator, use the **Share** link to share the script with your cluster administrator. 
- If you are a cluster administrator, click **Run script** to run the pre-installation check. Confirm that the script completes successfully.  


## Step 4. Set the deployment values
{: #set-deploy-values}

Override the default deployment values:

1. Enter a value for the consoleRoutePrefix parameter. This value is added as a subdomain to your OpenShfit Cluster Console URL so that you can access the {{site.data.keyword.cpd_full_notm}} web client. 
1. Specify the password for the default {{site.data.keyword.cpd_full_notm}} user (`admin`).


## Step 5. Install {{site.data.keyword.cpd_full_notm}}
{: #install-cloud-pak-for-data}

1. Ensure that you have assigned a license for {{site.data.keyword.cpd_full_notm}} to the deployment. 
1. Confirm that you have read and agree to the license agreements. 
1. Click **Install**.



## Next steps
{: #next-steps}

When the installation completes, you can access your {{site.data.keyword.cpd_full_notm}} deployment with the provided URL. 

Log in to the web client as `admin` using the password that you created in the preceding steps. 

For details on creating additional users, see [Managing users](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/com.ibm.icpdata.doc/zen/admin/users.html).

<!-- Add the topic to your `toc` file:


{:navgroup: .navgroup}
{:topicgroup: .topicgroup}

{: .toc subcollection="<Folder_name>" audience="oss" category="<category>" href="/docs/<folder_name>?topic=<subcollection>getting-started"}
<Cloud Pak Name>

    {: .navgroup id="learn"}
    getting-started.md

    {: .topicgroup}
    Related links
        [Link text](link URL)
    {: .navgroup-end}

    {: .navgroup id="reference"}
    Reference
    [Link text](link URL)
    {: .navgroup-end}
-->
