---

copyright:
  years: 2019, 2020
lastupdated: "2020-02-20"

keywords: "command line, getting started, {{site.data.keyword.cpd_short}}, {{site.data.keyword.cpd_full_notm}}, data, ai, analytics, data analytics, governance, data governance"

subcollection: cloud-pak-data

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}


# Using the command line interface in {{site.data.keyword.cpd_full_notm}}
{: #command-line}

You can use the Cloud Pak for Data command-line interface to install the Cloud Pak for Data control plane and any services that you want to run. 
You install Cloud Pak for Data on an IBM Cloud managed OpenShift cluster. 

The following commands can be used to install any service after 'oc login' to the cluster from a machine where the OpenShift CLI (oc) v4.3.18 and above compatible client with OpenShift cluster version is installed:

`./cpd-linux adm --apply --repo <repofile> --assembly <assembly>  --namespace <namespace> --accept-all-licenses`

`./cpd-linux --repo <repofile> --assembly <assembly>  --target-registry-password $(oc whoami -t) --target-registry-username $(oc whoami) --insecure-skip-tls-verify --cluster-pull-prefix image-registry.openshift-image-registry.svc:5000/<namespace> --transfer-image-to $(oc get route -n openshift-image-registry |tail -1|awk '{print $2}'/<namespace> --namespace <namespace> -c ibmc-file-gold-gid --accept-all-licenses`

For more information, see [Getting started with the CLI](https://docs.openshift.com/container-platform/4.3/cli_reference/openshift_cli/getting-started-cli.html).
