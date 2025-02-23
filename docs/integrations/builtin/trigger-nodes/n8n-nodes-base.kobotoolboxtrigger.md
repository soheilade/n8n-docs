---
title: KoBo Toolbox trigger
description: Documentation for the KoBo Toolbox trigger node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
contentType: integration
---

# KoBo Toolbox trigger

[KoBo toolbox](https://www.kobotoolbox.org/) is a field survey and data collection tool to design interactive forms to be completed offline from mobile devices. It's available both as a free cloud solution or as a self-hosted version.

/// note | Credentials
You can find authentication information for this node [here](/integrations/builtin/credentials/kobotoolbox/).
///
This node starts a workflow upon new submissions of a specified form. The trigger node handles the creation/deletion of the hook, so you don't need to do any setup in KoBo Toolbox.

It works the same way as the Get Submission operation in the [KoBoToolbox](/integrations/builtin/app-nodes/n8n-nodes-base.kobotoolbox/) node, including supporting the same reformatting options.
