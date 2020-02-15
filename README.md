# Remote-jupyter

local_user@local_host$ ssh merajahmed@10.237.22.140

remote_user@remote_host$ jupyter notebook --no-browser --port=8889

local_user@local_host$ ssh -N -f -L localhost:8888:localhost:8889 remote_user@remote_host
