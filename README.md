ansible-playbook rivalz_local_setup.yml -vv

docker exec -it rivalzNode0 /bin/bash -c "rivalz run"
docker exec -it rivalzNode0 /bin/bash -c "screen -dmS rivalzSession && screen -S rivalzSession -X stuff 'rivalz run\n'"

Remove screen with name
docker exec -it rivalzNode0 /bin/bash -c "screen -S rivalzSession -X quit"
