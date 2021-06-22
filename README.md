## Steps to use elasalert

1. start the env:

       source env/activate.fish

2. Test the rule:
        
       elastalert-test-rule --config config.yml rules/example_frequency.yaml

3. Send the alert to slack:

       python3 -m elastalert.elastalert --verbose --config config.yml --rule rules/example_frequency.yaml

4. Deactivate env:

        deactivate
---
    
## Create Dockerfile:


