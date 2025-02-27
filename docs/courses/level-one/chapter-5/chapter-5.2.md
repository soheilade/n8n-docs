---
contentType: tutorial
---

# 2. Inserting Data into Airtable

In this step of the workflow you will learn how to insert the data received using the HTTP Request node into Airtable using the *Airtable* node.

/// note | Spreadsheet nodes
You can replace the *Airtable* node with another spreadsheet app/service. For example, n8n also has nodes for [*Google Sheets*](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/){:target="_blank" .external} and [*Spreadsheet File*](/integrations/builtin/core-nodes/n8n-nodes-base.spreadsheetfile/){:target="_blank" .external}.
///

At this point, your workflow should look like this:

<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-2-workflow-with-airtable-node.png" alt="Workflow with the Airtable node" style="width:100%"><figcaption align = "center"><i>Workflow with the Airtable node</i></figcaption></figure>

If we're going to insert data into Airtable, we first need to set up a table there. To do this:

1. [Create an Airtable account](https://airtable.com/signup){:target="_blank" .external}.
2. In your Airtable workspace add a new base from scratch and name it, for example, *beginner course*.

	<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-2-create-airtable-base.png" alt="Create an Airtable base" style="width:100%"><figcaption align = "center"><i>Create an Airtable base</i></figcaption></figure>

3. In the beginner course base you have by default a *Table 1* with four fields: *Name, Notes, Assignee, and Status*.
These fields aren't relevant for us since they aren't in our orders data set. This brings us to the next point: the names of the fields in Airtable have to match the names of the columns in the node result.
  - Replace the four default table fields with the five column names from the data set, selecting **Number** field type for `orderID`, `customerID`, and `orderPrice`, and **Single line text** for `employeeName` and `orderStatus`.
  - Delete the 3 blank rows created by default.
  - Also, rename the table from *Table 1* to *orders* to make it easier to identify.

Now your table should look like this:

<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-2-orders-table.png" alt="Orders table in Airtable" style="width:100%"><figcaption align = "center"><i>Orders table in Airtable</i></figcaption></figure>

Now that the table is prepared let's return to the workflow in the Editor UI.

Add an ***Airtable node*** connected to the HTTP Request node.


In the *Airtable node* window, configure the following parameters:

- *Credential to connect with:*
	- Select 'Create new credential'
	- Keep the default option 'Connect using: Access Token' selected
	- *Access token:* Follow the instructions [here](/integrations/builtin/credentials/airtable/){:target="_blank" .external} to create your token.
Adding credentials for Airtable is similar to the HTTP Request node you configured in the previous chapter. However, the process of obtaining an API key for Airtable (and other apps/services) is different.
- *Resource:* Record
- *Operation:* Create. This operation will create the new record in the table.
- *Base:* You can pick your base from a list(e.g beginner course), URL or ID after authenticating. If you wish to use the Base ID, go to [Airtable's API page](https://airtable.com/developers/web/api/introduction){:target="_blank" .external} and find the relevant base (located at the bottom of the page). Then click the base title and you'll find the ID on that page.
- *Table:* orders
- *Mapping Column Mode:* Map automatically. In this mode, the incoming data fields are named the same as the columns in Airtable

Now execute the *Airtable* node and you should get the following result:

<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-2-airtable-node.png" alt="Airtable node results" style="width:100%"><figcaption align = "center"><i>Airtable node results</i></figcaption></figure>

All 30 data records will now appear in the orders table:

<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-2-airtable-records.png" alt="Imported records in the orders table" style="width:100%"><figcaption align = "center"><i>Imported records in the orders table</i></figcaption></figure>

## What's next?

**Nathan 🙋**: Wow, this automation is really useful! But this inserts all collected data from the HTTP Request node into Airtable. Remember that I actually need to insert only processing orders in the table and calculate the price of booked orders?

**You 👩‍🔧**: Sure, no problem. As a next step, I'll use a new node to filter the orders based on their status.
