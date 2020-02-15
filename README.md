# Remote-jupyter

merajahmed$ ssh merajahmed@10.237.22.140

merajahmed@vindhya:~$ jupyter notebook --no-browser --port=8889

local_user@local_host$ ssh -N -f -L localhost:8888:localhost:8889 remote_user@remote_host
