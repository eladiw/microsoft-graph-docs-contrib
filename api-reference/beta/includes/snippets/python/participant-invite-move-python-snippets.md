---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = InvitePostRequestBody(
	participants = [
		InvitationParticipantInfo(
			odata_type = "#microsoft.graph.invitationParticipantInfo",
			replaces_call_id = "a7ebfb2d-871e-419c-87af-27290b22e8db",
			participant_id = "7d501bf1-5ee4-4605-ba92-0ae4513c611c",
			identity = IdentitySet(
				odata_type = "#microsoft.graph.identitySet",
				user = Identity(
					odata_type = "#microsoft.graph.identity",
					id = "682b6c37-0729-4fab-ace6-d730d5d9137e",
					additional_data = {
							"identity_provider" : "AAD",
					}
				),
			),
		),
	]
	client_context = "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
)

result = await graph_client.communications.calls.by_call_id('call-id').participants.invite.post(body = request_body)


```