---
contentType: overview
---

# Integrations

n8n calls integrations nodes.

Nodes are the building blocks of workflows in n8n. They're an entry point for retrieving data, a function to process data, or an exit for sending data. The data process includes filtering, recomposing, and changing data. There can be one or several nodes for your API, service or app. You can connect multiple nodes, which allows you to create complex workflows.

## Built-in nodes

n8n includes a collection of built-in integrations. Refer to [Built-in nodes](/integrations/builtin/) for documentation on all n8n's built-in nodes.

## Community nodes

As well as using the built-in nodes, you can also install community-built nodes. Refer to [Community nodes](/integrations/community-nodes/) for more information.

## Credential-only nodes and custom operations

--8<-- "_snippets/integrations/credential-only-intro.md"

Refer to [Custom operations](/integrations/custom-operations/) for more information.

## Generic integrations

If you need to connect to a service where n8n doesn't have a node, or a credential-only node, you can still use the [HTTP Request](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) node. Refer to the node page for details on how to set up authentication and create your API call.

## Where to go next

* If you want to create your own node, head over to the [Creating Nodes](/integrations/creating-nodes/) section.
* Check out [Community nodes](/integrations/community-nodes) to learn about installing and managing community-built nodes.
* If you'd like to learn more about the different nodes in n8n, their functionalities and example usage, check out n8n's node libraries: [Core nodes](/integrations/builtin/core-nodes/), [Actions](/integrations/builtin/app-nodes/), and [Triggers](/integrations/builtin/trigger-nodes/).
* If you'd like to learn how to add the credentials for the different nodes, head over to the [Credentials](/integrations/builtin/credentials/) section.
