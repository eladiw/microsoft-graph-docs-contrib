---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = SectionGroup(
	display_name = "Section group name",
)

result = await graph_client.me.onenote.notebooks.by_notebook_id('notebook-id').section_groups.post(body = request_body)


```