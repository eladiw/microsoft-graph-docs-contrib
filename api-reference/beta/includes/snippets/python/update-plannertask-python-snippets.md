---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = PlannerTask(
	assignments = PlannerAssignments(
		additional_data = {
				"fbab97d0-4932-4511-b675-204639209557" : (
					odata_type = "#microsoft.graph.plannerAssignment",
					order_hint = "N9917 U2883!",
				),
		}
	),
	applied_categories = PlannerAppliedCategories(
		additional_data = {
				"category3" : True,
				"category4" : False,
		}
	),
	recurrence = PlannerTaskRecurrence(
		schedule = PlannerRecurrenceSchedule(
			pattern = RecurrencePattern(
				type = RecurrencePatternType.Daily,
				interval = 3,
			),
			pattern_start_date_time = "2022-02-22T02:10:33Z",
		),
	),
)

request_configuration = PlannerTaskRequestBuilder.PlannerTaskRequestBuilderPatchRequestConfiguration(
headers = {
		'Prefer' : "return=representation",
		'If-Match' : "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
}

)

result = await graph_client.planner.tasks.by_task_id('plannerTask-id').patch(body = request_body, request_configuration = request_configuration)


```