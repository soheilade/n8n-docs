---
title: Asana
description: Documentation for the Asana node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
contentType: integration
---

# Asana

Use the Asana node to automate work in Asana, and integrate Asana with other applications. n8n has built-in support for a wide range of Asana features, including creating, updating, deleting, and getting users, tasks, projects, and subtasks.

On this page, you'll find a list of operations the Asana node supports and links to more resources.

/// note | Credentials
Refer to [Asana credentials](/integrations/builtin/credentials/asana/) for guidance on setting up authentication. 
///

/// note | Examples and templates
For usage examples and templates to help you get started, take a look at n8n's [Asana integrations](https://n8n.io/integrations/asana/){:target="_blank" .external-link} list.
///

/// note | Update to 1.22.2 or above
Due to changes in Asana's API, some operations in this node stopped working on 17th January 2023. Upgrade to n8n 1.22.2 or above.
///

## Basic Operations

* Project
    * Create a new project
    * Delete a project
    * Get a project
    * Get all projects
    * Update a project
* Subtask
    * Create a subtask
    * Get all subtasks
* Task
    * Create a task
    * Delete a task
    * Get a task
    * Get all tasks
    * Move a task
    * Search for tasks
    * Update a task
* Task Comment
    * Add a comment to a task
    * Remove a comment from a task
* Task Tag
    * Add a tag to a task
    * Remove a tag from a task
* Task Project
    * Add a task to a project
    * Remove a task from a project
* User
    * Get a user
    * Get all users

## Example Usage

This workflow allows you to create a new task in Asana. You can also find the [workflow](https://n8n.io/workflows/478) on the website. This example usage workflow would use the following two nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Asana]()

The final workflow should look like the following image.

![A workflow with the Asana node](/_images/integrations/builtin/app-nodes/asana/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Asana node

1. First of all, you'll have to enter credentials for the Asana node. You can find out how to do that [here](/integrations/builtin/credentials/asana/).
2. Select your workspace from the *Workspace* dropdown list.
3. Enter the name of the task in the *Name* field.
4. Click on *Execute Node* to run the workflow.





