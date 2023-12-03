---

copyright:
  years: 2019, 2023
lastupdated: "2023-12-04"

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
* Some services can be installed by creating a catalog source and an operator subscription for each service. For general information and prerequisites, see [Installing IBM Cloud Pak for Data](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/install/install.html). To use this method, you must:
   * Use the Red Hat OpenShift command-line interface (oc CLI) to connect to the cluster. For more information, see [Connecting to the cluster from the CLI](https://cloud.ibm.com/docs/openshift?topic=openshift-access_cluster#access_oc_cli). 
   * Create an operator subscription for each service that you plan to install. For more information, see [Creating OLM objects for an express installation](https://www.ibm.com/docs/SSQNUZ_4.7.x/cpd/install/install-platform-express-olm.html).

Use the links in the following table to learn how to install each of these services.

|Service          |Install from the Cloud Pak for Data installation page    |Install by using the CLI|
|:------------- |:-----------------------------------------------------------------:| :-----------:|
|[Analytics Engine Powered by Apache Spark](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/spark.html)                                                         | ✓ | ✓ |
|[AI Factsheets](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/aifact.html)                                                                                   | ✓ | ✓ |
|[Cognos Analytics](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/ca.html)                                                                                    | |  ✓  |
|[Cognos Dashboards](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/idash.html)                                                                                | ✓ | ✓ |
|[Data Refinery](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/dr.html)| See Watson Knowledge Catalog or Watson Studio |See Watson Knowledge Catalog or Watson Studio |
|[DataStage](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/ds.html)                                                                                           | |  ✓  |
|[Db2 Big SQL](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/bigsql.html)                                                                                     | |  ✓  |
|[Db2 Data Gate](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/dg.html)                                                                                       | ✓ | ✓ |
|[Db2 Data Management Console](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/dmc.html)                                                                        | ✓ | ✓ |
|[Db2 Warehouse](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/db2wh.html)                                                                                    | ✓ | ✓ |
|[Db2](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/db2oltp.html)                                                                                              | | ✓ |
|[Decision Optimization](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/do.html)                                                                               | |  ✓  |
|[Execution Engine for Apache Hadoop](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/hadoopaddon.html)                                                         | |  ✓  |
|[IBM Match 360](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/mdc.html)                                                                                      | |  ✓  |
|[OpenPages](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/openpages.html)                                                                                    | |  ✓  |
|[Planning Analytics](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/pa.html)                                                                                  | |  ✓  |
|[RStudio Runtimes](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/rstudio.html)                                                                               | ✓ | ✓ |
|[SPSS Modeler](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/spssmodeler.html)                                                                               | |  ✓  |
|[Watson Knowledge Catalog](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/wkc.html)                                                                           | ✓ | ✓ |
|[Watson Machine Learning](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/wml.html)                                                                            | ✓ | ✓ |
|[Watson OpenScale](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/aiopenscale.html)                                                                           | ✓ | ✓ |
|[Watson Pipeines](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/wsp.html)                                                                                      | | ✓ |
|[Watson Query](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/dv.html)                                                                                        | ✓ | ✓ |
|[Watson Studio](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/wsl.html)                                                                                      | ✓ | ✓ |
|[Watson Studio Runtimes](https://www.ibm.com/docs/SSQNUZ_4.7.x/svc-welcome/jupyter.html)                                                                         |  |  ✓ |
{: caption="Table 1. Methods to install Cloud Pak for Data" caption-side="bottom"}
