# Test case for data sunrise : principal-checks and schema 

```
	Background:
		
		Given I can parse "/arm_dist/azuredeploy.json" json
	
	Scenario: Key contains a value.
		
		When $schema is the key on template file
		
		Then Its value should contain 2015-01-01/deploymentTemplate.json

		
		When parameters.adminUsername.value is the key on params file
		Then Its value should contain datasunrise

		When parameters.adminPassword.value is the key on params file
		Then Its value should contain Ashpassword123
