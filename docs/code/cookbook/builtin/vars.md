---
description: Access your environment's custom variables.
contentType: reference
---

# `vars`

/// info | Feature availability
* Available on Self-hosted Enterprise and Pro and Enterprise Cloud plans.
* You need access to the n8n instance owner account to create variables.
///	

`vars` contains all [Variables](/code/variables/) for the active environment. It's read-only: you can access variables using `vars`, but must set them using the UI.

=== "JavaScript"
	```js
	// Access a variable
	$vars.<variable-name>
	```
=== "Python"
	```python
	# Access a variable
	_vars.<variable-name>
	```

/// note | `vars` and `env`
`vars` gives access to user-created variables. It's part of the [Environments](/source-control-environments/) feature. `env` gives access to the [configuration environment variables](/hosting/environment-variables/environment-variables/) for your n8n instance. 
///
