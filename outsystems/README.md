
# Test cases for outsystems

```
		Background:
		Given I can parse "/arm_dist/azuredeploy.json" json
	Scenario: Key has/not a specific value.
		When $schema is the key on template file
		Then https://schema.management.azure.com/schemas/2015-01-01/deploymentTemplate.json# yes be its value

		When contentVersion is the key on template file
		Then 1.0.0.0 yes be its value

		When parameters.adminUserName.value is the key on params file
		Then  testuser yes be its value

		When parameters.adminPassword.value is the key on params file
		Then Qwerty12 yes be its value

		
