---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)


result = await graph_client.identity_governance.acce_reviews.history_definitions.by_history_definition_id('accessReviewHistoryDefinition-id').instances.by_instance_id('accessReviewHistoryInstance-id').generate_download_uri.post()


```