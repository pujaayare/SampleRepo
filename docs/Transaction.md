---
layout: default
title: Transaction
nav_order: 12
---
# Create Transaction:
 *  Create transaction: - Right-click on the **FactoCloudConnect** project resource in the Project browser tree

 ![](../../assets/images/newtransaction.png)
{: style="text-align:center;"}
 *  On the Form, select connector Type, either Producer or Consumer.
**Producer:** This will push data to the selected Connector. FactoCloudConnect uses ActiveMQ Artemis Server.
**Consumer:** This will receive/consume data from the Connector source and overwrite to tag values.
**Note:** It is essential to save the project after creating a transaction. Failure to do so may result in the resource not being available later. 
 * **Producer:** 

 ![](../../assets/images/Producer.png)
{: style="text-align:center;"}
 *  Select a connector from the list of connectors available from the dropdown.
There are at present three connectors available: Kafka, EventHub, Database, ElasticSearch, and InfluxDb.

![](../../assets/images/kafkaconnector.png)
{: style="text-align:center;"}
**Note:** In the case of the Database, the available connections can be chosen from the default connections section of the config page.
 *  Select connection (if the connection list is empty then need to create connections on the Ignition gateway under the “config” section, FactoCloudConnect  Menu – Connectors)

 ![](../../assets/images/connection.png)
{: style="text-align:center;"}
 *  Once a connection is created,  then selecting that connection from the dropdown will autofill the relevant fields on the form.

 ![](../../assets/images/connection1.png)
{: style="text-align:center;"}
 *  Default values of Config and Trigger sections can be customized
 **Consumer:** This will receive/consume data from the Connector source and overwrite to tag values
 
 ![](../../assets/images/consumer.png)
{: style="text-align:center;"}
 Select ‘Connector’ from dropdown connector dropdown

  ![](../../assets/images/consumerconnector.png)
{: style="text-align:center;"}
 Select ‘Connection’ from the connection dropdown 
 
   ![](../../assets/images/consumerconnection.png)
{: style="text-align:center;"}
 Then see all values properly display in all fields
 Note: If we Produce a message using any Data Format (Ex:- JSON, CSV, AVRO, and SPARKPLUGB) then we should consume the message using the same Data Format.

   ![](../../assets/images/consumerfullscreen.png)
{: style="text-align:center;"}
Note: Supported Tag DataTypes are  Short,Integer,Long,Float,Double,Boolean,String.
 *  Inside the Tag Browser Tree, data tags will have to be added to the Producer Tags folder under the respective Transaction folder.

 ![](../../assets/images/produerTags.png)
{: style="text-align:center;"}
 *  Tags are available in Four forms: Control Tags, Producer Tags, Consumer Tags, and Trigger tags.
 
 ![](../../assets/images/folders.png)
{: style="text-align:center;"}
 **Control Tags:** These tags store “Transaction State” related information. 

  ![](../../assets/images/controltags.png)
{: style="text-align:center;"}
 **ProducerTags:** These tags hold the information which requires to be pushed or transferred to the target instance.

 ![](../../assets/images/producertags.png)
{: style="text-align:center;"}
 **TriggerTags:** These tags are configured to push data based on value change when the selected trigger type is not “Timer”.

 ![](../../assets/images/triggertags.png)
{: style="text-align:center;"}
 **ConsumerTags:** These tags are created and hold the consumed data when a consumer transaction runs.

  ![](../../assets/images/consumertag.png)
{: style="text-align:center;"}
 Click on “Submit” (save successfully with the 'ok' button popup) and then the “Start” button.
 At the bottom right corner of the screen, the user can see the two-step, the "Running..." indication and "Active MQ server running...”



