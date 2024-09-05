##Install - 
ansible-playbook rivalz_local_setup.yml -vv

##Run once and setup node - 
docker exec -it rivalzNode0 /bin/bash -c "rivalz run"

##Run node - 
docker exec -it rivalzNode0 /bin/bash -c "screen -dmS rivalzSession && screen -S rivalzSession -X stuff 'rivalz run\n'"

##Remove screen with name - 
docker exec -it rivalzNode0 /bin/bash -c "screen -S rivalzSession -X quit"
