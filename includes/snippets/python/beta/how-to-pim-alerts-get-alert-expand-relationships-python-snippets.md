---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = UnifiedRoleManagementAlertRequestBuilder.UnifiedRoleManagementAlertRequestBuilderGetQueryParameters(
		expand = ["*"],
)

request_configuration = UnifiedRoleManagementAlertRequestBuilder.UnifiedRoleManagementAlertRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.identity_governance.role_management_alerts.alerts.by_alert_id('unifiedRoleManagementAlert-id').get(request_configuration = request_configuration)


```