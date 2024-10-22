---

copyright:
  years: 2019, 2024
lastupdated: "2024-10-09"

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
* Some services can be installed by creating a catalog source and an operator subscription for each service. For general information and prerequisites, see [Installing IBM Cloud Pak for Data](https://www.ibm.com/docs/SSQNUZ_latest/cpd/install/install.html). To use this method, you must:
   * Use the Red Hat OpenShift command-line interface (oc CLI) to connect to the cluster. For more information, see [Connecting to the cluster from the CLI](https://cloud.ibm.com/docs/openshift?topic=openshift-access_cluster#access_oc_cli).
   * Create an operator subscription for each service that you plan to install. For more information, see [Installing an instance of IBM Cloud Pak for Data](https://www.ibm.com/docs/SSQNUZ_latest/cpd/install/install-platform.html).

Use the links in the following table to learn how to install each of these services.

|Service          |Install from the Cloud Pak for Data installation page    |Install by using the CLI|
|:------------- |:-----------------------------------------------------------------:| :-----------:|
|[Analytics Engine Powered by Apache Spark](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/spark.html)                                                         | ✓ | ✓ |
|[AI Factsheets](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/aifact.html)                                                                                   | ✓ | ✓ |
|[Cognos Analytics](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/ca.html)                                                                                    | |  ✓  |
|[Cognos Dashboards](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/idash.html)                                                                                | ✓ | ✓ |
|[Data Refinery](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/dr.html)| See Watson Knowledge Catalog or Watson Studio |See Watson Knowledge Catalog or Watson Studio |
|[DataStage](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/ds.html)                                                                                           | |  ✓  |
|[Db2 Big SQL](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/bigsql.html)                                                                                     | |  ✓  |
|[Db2 Data Management Console](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/dmc.html)                                                                        | ✓ | ✓ |
|[Db2 Warehouse](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/db2wh.html)                                                                                    | ✓ | ✓ |
|[Db2](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/db2oltp.html)                                                                                            | | ✓ |
|[Decision Optimization](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/do.html)                                                                               | |  ✓  |
|[IBM Match 360](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/mdc.html)                                                                                      | |  ✓  |
|[MANTA Automated Data Lineage](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/manta.html)                                                                     | ✓ | ✓ |
|[OpenPages](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/openpages.html)                                                                                    | |  ✓  |
|[Planning Analytics](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/pa.html)                                                                                  | |  ✓  |
|[RStudio Runtimes](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/rstudio.html)                                                                               | ✓ | ✓ |
|[SPSS Modeler](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/spssmodeler.html)                                                                               | |  ✓  |
|[Watson Assistant](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/watsonassist.html)                                                                          | ✓ | ✓ |
|[Watson Discovery](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/watsondisc.html)                                                                             | ✓ | ✓ |
|[Watson Knowledge Catalog](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/wkc.html)                                                                           | ✓ | ✓ |
|[Watson Machine Learning](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/wml.html)                                                                            | ✓ | ✓ |
|[Watson OpenScale](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/aiopenscale.html)                                                                           | ✓ | ✓ |
|[Watson Pipelines](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/wsp.html)                                                                                   | | ✓ |
|[Watson Speech](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/wstt.html)                                                                                     | ✓| ✓ |
|[Watson Query](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/dv.html)                                                                                        | ✓ | ✓ |
|[Watson Studio](https://www.ibm.com/docs/SSQNUZ_latest/svc-welcome/wsl.html)                                                                                      | ✓ | ✓ |
{: caption="Methods to install Cloud Pak for Data" caption-side="bottom"}
