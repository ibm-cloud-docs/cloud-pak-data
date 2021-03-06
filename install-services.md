---

copyright:
  years: 2019, 2020, 2021
lastupdated: "2020-11-20"

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


# Installing services
{: #install-services}

If you deploy {{site.data.keyword.cpd_full_notm}} on IBM Cloud, you can install a subset of the services that are available in the {{site.data.keyword.cpd_short}} services catalog.

You can install services using two different methods. The supported methods depend on the services that you want to install:

* Some services can be installed from the [{{site.data.keyword.cpd_short}} installation page](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global) in the IBM Cloud catalog.
* Some services can be installed by creating an operator subscription for services. To use this method, you must:
   * Use the Red Hat OpenShift command-line interface (oc CLI) to connect to the cluster. For more information, see [Connecting to the cluster from the CLI](https://cloud.ibm.com/docs/openshift?topic=openshift-access_cluster#access_oc_cli). 
   * Creating an operator subscription for services. For more information, see [Creating an operator subscription for services](https://www.ibm.com/docs/en/SSQNUZ_4.0/cpd/install/preinstall-operator-subscriptions.html).

Use the links in the following table to learn how to install each of these services.

|Service 	      |Install from the Cloud Pak for Data installation page 	|Install by using the CLI|
|:------------- |:-----------------------------------------------------------------:| :-----------:|
|[Analytics Engine Powered by Apache Spark](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-analytics-engine-powered-by-apache-spark)                                           | 	✓ | 	✓ |
|[Cognos Analytics](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-cognos-analytics) 	                                                                |     |  ✓  |
|[Cognos Dashboards](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-cognos-dashboards)                                                                 | 	✓ | 	✓ |
|[Data Refinery](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-data-refinery)|	See Watson Knowledge Catalog or Watson Studio |	See Watson Knowledge Catalog or Watson Studio |
|[Data Virtualization](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-data-virtualization)                                                                | 	✓ | 	✓ |
|[DataStage Edition](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-datastage)                                                                  |     |  ✓  |
|[Db2 Big SQL](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-db2-big-sql)                                                                        |     |  ✓  |
|[Db2 Data Gate](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-db2-data-gate)                                                                        |  ✓  |  ✓  |
|[Db2 Data Management Console](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-db2-data-management-console)                                                                        |  ✓  |  ✓  |
|[Db2 Warehouse](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-db2-warehouse)                                                                      | 	✓ | 	✓ |
|[Db2 ](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-db2)                                                                      | 	  | 	✓ |
|[Decision Optimization](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-decision-optimization)                                                              |     |  ✓  |
|[Execution Engine for Apache Hadoop](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-execution-engine-apache-hadoop)                                                 |     |  ✓  |
|[Jupyter Notebooks with Python 3.7 for GPU](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-jupyter-python-37-gpu)                                        	|     |  ✓  |
|[Jupyter Notebooks with R 3.6](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-jupyter-notebooks-r-36)                                                      |     |  ✓  |
|[MongoDB](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-mongodb)                                                                            |     |  ✓  |
|[RStudio Server with R 3.6](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-rstudio-server-r-36)                                                         | 	✓ | 	✓ |
|[SPSS Modeler](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-spss-modeler)                                                                       |     |  ✓  |
|[Scheduling](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=tasks-setting-up-scheduling-service)                                                                       |   ✓ |  ✓  |
|[Watson Knowledge Catalog](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-watson-knowledge-catalog)                                                           | 	✓ | ✓  |
|[Watson Machine Learning](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-watson-machine-learning)                                                            | 	✓ | 	✓ |
|[Watson Machine Learning Accelerator](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-watson-machine-learning-accelerator)                                                            | 	✓ | 	✓ |
|[Watson OpenScale](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-watson-openscale)                                                                   | 	✓ | 	✓ |
|[Watson Studio](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.0?topic=services-watson-studio)                                                                      | 	✓ | 	✓ |

A * indicates that the service is supported only on bare metal worker nodes with extra local storage for software-defined storage (SDS). These services also require [Portworx Enterprise](https://cloud.ibm.com/catalog/services/portworx-enterprise) storage. You must create a new worker pool that contains the bare metal servers required for Watson AI services.
