---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW VERSION OF THE SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestConfiguration = new UsersRequestBuilderGetRequestConfiguration();
$queryParameters = UsersRequestBuilderGetRequestConfiguration::createQueryParameters();
$queryParameters->top = 5;
$queryParameters->skiptoken = "skiptoken=RFNwdAIAAQAAAD8...AAAAAAAA";
$requestConfiguration->queryParameters = $queryParameters;


$result = $graphServiceClient->users()->get($requestConfiguration)->wait();

```