---
layout: default
title: Prerequisites of the module
nav_order: 4
---
# Prerequisites of the module
 *  On the Ignition gateway, the user needs to create a real-time  standard tag provider named FactoCloudConnect. This provider stores the default settings.
 *  Once the tag provider is created, the module file will have to be uploaded on Ignition

 ![](../../assets/images/moduleinstallation.png)
{: style="text-align:center;"}
 *  FactoCloudConnect Producer uses  Apache ActiveMQ Artemis Server. It is an open-source asynchronous messaging system. If the user wants to change any of the default settings, these can be changed via 
 the Queue management option

  ![](../../assets/images/queuemanagement.png)
{: style="text-align:center;"}
 *  After uploading the module, the next step is to create a connection for the connectors 

  ![](../../assets/images/afterinstallation.png)
{: style="text-align:center;"}
 *  On choosing “Create new Connector..”, the category for the connector needs to be specified.
 
 ![](../../assets/images/connectors.png)
{: style="text-align:center;"}
 *  Once the proper category is chosen, the required information can be passed to complete connector creation.

 ![](../../assets/images/kafkaconnection.png)
{: style="text-align:center;"}

