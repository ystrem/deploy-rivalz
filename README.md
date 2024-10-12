##Install - 
ansible-playbook rivalz_local_setup.yml -vv or ansible-playbook rivalz_local_setup.yml --ask-become-pass

##Run once and setup node - 
docker exec -it rivalzNode0 /bin/bash -c "rivalz run"

##Run node - 
docker exec -it rivalzNode0 /bin/bash -c "screen -dmS rivalzSession && screen -S rivalzSession -X stuff 'rivalz run\n'"

##Remove screen with name - 
docker exec -it rivalzNode0 /bin/bash -c "screen -S rivalzSession -X quit"

If you like it TipMe
EVM : 0x276366e2436E9D062BAAbF58755A8Ae2D256b996
SOL : EA3QSrDy3EBX1uq3w5NP2AJSsXDxi9LiYkjCjNHyYfhP
