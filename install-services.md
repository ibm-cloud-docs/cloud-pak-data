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

You can install services by using two different methods. The supported methods depend on the services that you want to install:

* Some services can be installed from the [{{site.data.keyword.cpd_short}} installation page](https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global) in the IBM Cloud catalog.
* Some services can be installed by running the {{site.data.keyword.cpd_short}} command-line interface (CLI). To use this method, you must:
   * Use the Red Hat OpenShift command-line interface (oc CLI) to connect to the cluster. For more information, see [Connecting to the cluster from the CLI](https://cloud.ibm.com/docs/openshift?topic=openshift-access_cluster#access_oc_cli). 
   * Download and install {{site.data.keyword.cpd_short}} CLI (cpd-cli). For more information, see [Obtaining the installation files](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/cpd/install/installation-files.html).

Use the links in the following table to learn how to install each of these services.

|Service 	      |Install from the Cloud Pak for Data installation page 	|Install by using the CLI|
|:------------- |:-----------------------------------------------------------------:| :-----------:|
|[Analytics Engine Powered by Apache Spark](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/spark.html)                                           | 	✓ | 	✓ |
|[Cognos Analytics](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/ca.html) 	                                                                |     |  ✓  |
|[Cognos Dashboards](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/cde.html)                                                                 | 	✓ | 	✓ |
|[Data Refinery](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/dr.html)|	See Watson Knowledge Catalog or Watson Studio. |	See Watson Knowledge Catalog or Watson Studio. |
|[Data Virtualization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/dv.html)                                                                | 	✓ | 	✓ |
|[DataStage Edition](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/ds.html)                                                                  |     |  ✓  |
|[Db2 Big SQL](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/bigsql.html)                                                                        |     |  ✓  |
|[Db2 Data Gate](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/dg.html)                                                                        |  ✓  |  ✓  |
|[Db2 Data Management Console](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/dmc.html)                                                                        |  ✓  |  ✓  |
|[Db2 for z/OS](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/db2z.html)                                                                       |     |  ✓  |
|[Db2 Warehouse](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/db2wh.html)                                                                      | 	✓ | 	✓ |
|[Decision Optimization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/do.html)                                                              |     |  ✓  |
|[Execution Engine for Apache Hadoop](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/hadoopaddon.html)                                                 |     |  ✓  |
|[Financial Crimes Insight](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/cpd/svc/fci/fci-install.html)                                                           |     |  ✓  |
|[Jupyter Notebooks with Python 3.6 for GPU](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/gpupy36.html)                                        	|     |  ✓  |
|[Jupyter Notebooks with R 3.6](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/r36.html)                                                      |     |  ✓  |
|[MongoDB](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/mongodb.html)                                                                            |     |  ✓  |
|[RStudio Server with R 3.6](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/rstudio.html)                                                         | 	✓ | 	✓ |
|[SPSS Modeler](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/spssmodeler.html)                                                                       |     |  ✓  |
|[Streams](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/streams.html)                                                                            | 	✓ |  ✓  |
|[Streams Flows](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/cpd/svc/streams/installing-streams-flows.html)                                                                      | 	✓ |  ✓ |
|[Watson AIOps](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/aiops.html)                                                                       |     |  *  |
|[Watson Assistant](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/watsonassist.html)                                                                   |     |  *  |
|[Watson Assistant for Voice Interaction](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/wavi.html)                                             |     |  *  |
|[Watson Discovery](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/watsondisc.html)                                                                   |     |  *  |
|[Watson Knowledge Catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/wkc.html)                                                           | 	✓ | ✓  |
|[Watson Knowledge Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/watsonks.html)                                                            |     |  *  |
|[Watson Language Translator](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/wlt.html)                                                         |     |  *  |
|[Watson Machine Learning](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/wml.html)                                                            | 	✓ | 	✓ |
|[Watson OpenScale](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/aiopenscale.html)                                                                   | 	✓ | 	✓ |
|[Watson Speech to Text](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/wstt.html)                                                              |     |  *  |
|[Watson Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/wsl.html)                                                                      | 	✓ | 	✓ |
|[Watson Text to Speech](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_latest/svc-welcome/wtts.html)                                                              |     |  *  |

A * indicates that the service is supported only on bare metal worker nodes with extra local storage for software-defined storage (SDS). These services also require [Portworx Enterprise](https://cloud.ibm.com/catalog/services/portworx-enterprise) storage. You must create a new worker pool that contains the bare metal servers that are required for Watson AI services.

