---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = CustomSecurityAttributeDefinition(
	attribute_set = "Engineering",
	description = "Target completion date",
	is_collection = False,
	is_searchable = True,
	name = "ProjectDate",
	status = "Available",
	type = "String",
	use_pre_defined_values_only = False,
)

result = await graph_client.directory.custom_security_attribute_definitions.post(body = request_body)


```