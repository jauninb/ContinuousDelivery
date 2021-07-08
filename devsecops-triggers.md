---

copyright:
  years: 2021
lastupdated: "2021-06-30"

keywords: DevSecOps, triggers

subcollection: ContinuousDelivery

---

{:shortdesc: .shortdesc}
{:table: .aria-labeledby="caption"}
{:external: target="_blank" .external}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:download: .download}
{:help: data-hd-content-type='help'}
{:support: data-reuse='support'}

# Triggers
{: #cd-devsecops-triggers}

DevSecops continuous integration and continuous delivery pipelines provide a set of default triggers.
{:shortdesc}

|Pipeline |Name	|Description |State |
|:----------|:------------------------------|:------------------|:----------|
|Pull request		|Git PR Trigger		|Runs the pull request pipeline on pull requests within the Application Repository.			|Enabled			|
|Pull request 		|Manual Trigger 		|Runs the pull request pipeline on a specified commit or branch, on demand.			|Enabled			|
|Continuous integration		|Git CI Timed Trigger		|Runs the continuous integration pipeline on the `master` branch of the Application Repository every day at 4 AM. |Disabled			|
|Continuous integration		|Git CI Trigger		|Runs the continuous integration pipeline when a commit is pushed to the master branch of the Application Repository.	|Enabled			|
|Continuous integration		|Manual Trigger 		|Runs the continuous integration pipeline on a specified commit or branch, on demand.		|Enabled			|
|Continuous delivery		|Git CD Timed Trigger		|Runs the continuous delivery pipeline every day at 4 AM.	|Disabled			|
|Continuous delivery		|Git CD Trigger		|Runs the continuous delivery pipeline when a commit is pushed to the `target-environment` branch of the Inventory.	|Disabled			|
|Continuous delivery		|Manual CD Trigger		|Runs the continuous delivery pipeline on the `target-environment` branch of the Inventory, on demand.	|Enabled			|
|Continuous delivery		|Manual Promotion Trigger		|Runs the promotion pipeline to promote inventory changes from the `source-environment` branch to the `target-environment` branch.	|Enabled			|
{: caption="Table 1. Triggers" caption-side="top"}

You can [add triggers](/docs/ContinuousDelivery?topic=ContinuousDelivery-cd-devsecops-add-pipeline-triggers) to the set of default triggers.
{: tip}
