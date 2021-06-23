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

1. Remove dangling images from docker build: 

       sudo docker rmi $(sudo docker images -f “dangling=true” -q)

2. Get inside docker container:

    1. Get container: 
            
           sudo docker ps

    2. Get inside container: 
        
           sudo docker exec -it <container-id> /bin/bash
13.71.110.1

sudo docker build --build-arg host=13.71.110.1 -t elastalert:1.0 ./DockerFiles/