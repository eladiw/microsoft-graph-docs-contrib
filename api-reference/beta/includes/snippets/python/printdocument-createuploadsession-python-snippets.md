---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = CreateUploadSessionPostRequestBody(
	properties = PrintDocumentUploadProperties(
		document_name = "TestFile.pdf",
		content_type = "application/pdf",
		size = 4533322,
	),
)

result = await graph_client.print.shares.by_share_id('printerShare-id').jobs.by_job_id('printJob-id').documents.by_document_id('printDocument-id').create_upload_session.post(body = request_body)


```