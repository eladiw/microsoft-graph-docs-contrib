---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)


result = await graph_client.employee_experience.learning_providers.by_learning_provider_id('learningProvider-id').learning_contents.by_learning_content_id('learningContent-id').get()


```