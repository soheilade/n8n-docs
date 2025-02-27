---
title: Mocean
description: Documentation for the Mocean node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
contentType: integration
---

# Mocean

Use the Mocean node to automate work in Mocean, and integrate Mocean with other applications. n8n has built-in support for a wide range of Mocean features, including sending SMS, and voice messages. 

On this page, you'll find a list of operations the Mocean node supports and links to more resources.

/// note | Credentials
Refer to [Mocean credentials](/integrations/builtin/credentials/mocean/) for guidance on setting up authentication. 
///
/// note | Examples and templates
For usage examples and templates to help you get started, take a look at n8n's [Mocean integrations](https://n8n.io/integrations/mocean/){:target="_blank" .external-link} list.
///


## Basic Operations

* SMS
    * Send SMS/Voice message
* Voice
    * Send SMS/Voice message


## Example Usage

This workflow allows you to send an SMS using the Mocean node. You can also find the [workflow](https://n8n.io/workflows/667) on n8n.io. This example usage workflow would use the following nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Mocean]()

The final workflow should look like the following image.

![A workflow with the Mocean node](/_images/integrations/builtin/app-nodes/mocean/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.


### 2. Mocean node

1. First of all, you'll have to enter credentials for the Mocean node. You can find out how to do that [here](/integrations/builtin/credentials/mocean/).
2. Enter the sender ID in the ***From*** field.
3. Enter the receivers' number in the ***To*** field.
4. Enter the message in the ***Message*** field.
5. Click on ***Test step*** to run the node.

![Using the Mocean node to send an SMS](/_images/integrations/builtin/app-nodes/mocean/mocean_node.png)

