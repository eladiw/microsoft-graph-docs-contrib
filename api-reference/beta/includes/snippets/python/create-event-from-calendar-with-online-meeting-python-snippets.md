---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = Event(
	subject = "Let's go for lunch",
	body = ItemBody(
		content_type = BodyType.Html,
		content = "Does next month work for you?",
	),
	start = DateTimeTimeZone(
		date_time = "2019-03-10T12:00:00",
		time_zone = "Pacific Standard Time",
	),
	end = DateTimeTimeZone(
		date_time = "2019-03-10T14:00:00",
		time_zone = "Pacific Standard Time",
	),
	location = Location(
		display_name = "Harry's Bar",
	),
	attendees = [
		Attendee(
			email_address = EmailAddress(
				address = "adelev@contoso.onmicrosoft.com",
				name = "Adele Vance",
			),
			type = AttendeeType.Required,
		),
	]
	is_online_meeting = True,
	online_meeting_provider = OnlineMeetingProviderType.TeamsForBusiness,
)

result = await graph_client.me.calendars.by_calendar_id('calendar-id').events.post(body = request_body)


```