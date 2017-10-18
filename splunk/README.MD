
# Test case for splunk 1

  ```
  	
	Background:
		Given I can parse \"/arm_dist/azuredeploy.json\" json
	Scenario: Key is/not Present.
		Then  $schema yes present in the template file
		Then  contentVersion yes present in the template file
	   
    Then  parameters.clientAdminUsername.value yes present in the params file
	
