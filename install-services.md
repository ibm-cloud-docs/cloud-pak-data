---

copyright:
  years: 2019, 2020
lastupdated: "2020-02-20"

keywords: "adding services, getting started, {{site.data.keyword.cpd_short}}, {{site.data.keyword.cpd_full_notm}}, data, ai, analytics, data analytics, governance, data governance"

subcollection: 




-pak-data

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



You can install services in different ways. The supported methods depend on the services that you want to install:

* Some services can be installed from the ({{site.data.keyword.cpd_short}} installation page)[https://cloud.ibm.com/catalog/content/ibm-cp-datacore-6825cc5d-dbf8-4ba2-ad98-690e6f221701-global] in the IBM Cloud catalog.
* Some services can be installed by running the {{site.data.keyword.cpd_short}} command-line interface.

|Service 	      |Install from the Cloud Pak for Data installation page 	|Install by using the CLI|
|:------------- |:-----------------------------------------------------------------:| :-----------:|
|[Analytics Engine Powered by Apache Spark](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/spark.html)                                           | 	✓ | 	✓ |
|[Cognos Analytics](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/ca.html) 	                                                                |     |  ✓  |
|[Cognos Dashboards](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/dashboard-svc.html)                                                                 | 	✓ | 	✓ |
|[Data Refinery](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/dr.html)|	See Watson Knowledge Catalog or Watson Studio |	See Watson Knowledge Catalog or Watson Studio |
|[Data Virtualization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/dv.html)                                                                | 	✓ | 	✓ |
|[DataStage Edition](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/ds.html)                                                                  |     |  ✓  |
|[Db2 Big SQL](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/bigsql.html)                                                                        |     |  ✓  |
|[Db2 for z/OS](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/db2z.html)                                                                       |     |  ✓  |
|[Db2 Warehouse](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/db2wh.html)                                                                      | 	✓ | 	✓ |
|[Decision Optimization](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/do.html)                                                              |     |  ✓  |
|[Execution Engine for Apache Hadoop](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/hadoopaddon.html)                                                 |     |  ✓  |
|[Financial Crimes Insight](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/fci/fci-install.html)                                                           |     |  ✓  |
|[Jupyter Notebooks with Python 3.6 for GPU](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/gpupy36.html)                                        	|     |  ✓  |
|[Jupyter Notebooks with R 3.6](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/r36.html)                                                      |     |  ✓  |
|[MongoDB](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/mongodb.html)                                                                            |     |  ✓  |
|[Open Source Management](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/osg.html)                                                             | 	✓ | 	✓ |
|[RStudio Server with R 3.6](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/rstudio.html)                                                         | 	✓ | 	✓ |
|[SPSS Modeler](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/spssmodeler.html)                                                                       |     |  ✓  |
|[Streams](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/streams.html)                                                                            | 	✓ |  ✓  |
|[Streams Flows](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/streams/installing-streams-flows.html)                                                                      | 	✓ |  ✓ |
|[Watson AIOps](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/cpd/svc/ai-svc.html)                                                                       |     |  *  |
|[Watson Assistant](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/watsonassist.html)                                                                   |     |  *  |
|[Watson Assistant for Voice Interaction](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wavi.html)                                             |     |  *  |
|[Watson Discovery](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/watsondisc.html)                                                                   |     |  *  |
|[Watson Knowledge Catalog](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wkc.html)                                                           | 	✓ | ✓  |
|[Watson Knowledge Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/watsonks.html)                                                            |     |  *  |
|[Watson Language Translator](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wlt.html)                                                         |     |  *  |
|[Watson Machine Learning](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wml.html)                                                            | 	✓ | 	✓ |
|[Watson OpenScale](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/aiopenscale.html)                                                                   | 	✓ | 	✓ |
|[Watson Speech to Text](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wstt.html)                                                              |     |  *  |
|[Watson Studio](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wsl.html)                                                                      | 	✓ | 	✓ |
|[Watson Text to Speech](https://www.ibm.com/support/producthub/icpdata/docs/content/SSQNUZ_current/svc-welcome/wtts.html)                                                              |     |  *  |

A * indicates that the service is supported only on bare metal worker nodes with extra local storage for SDS. These services also require (Portworx Enterprise)[https://cloud.ibm.com/catalog/services/portworx-enterprise] storage. You must create a new worker pool that contains the bare metal servers required for Watson AI services.

