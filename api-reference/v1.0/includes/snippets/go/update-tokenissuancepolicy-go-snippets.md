---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewTokenIssuancePolicy()
definition := []string {
	"definition-value",

}
requestBody.SetDefinition(definition)
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName) 
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault) 

graphClient.Policies().TokenIssuancePoliciesById("tokenIssuancePolicy-id").Patch(context.Background(), requestBody, nil)


```