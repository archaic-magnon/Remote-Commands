# Remote-jupyter
#### Run jupyter on server and access it on local browser
<hr/>

##### Merajs-MacBook-Air:~ merajahmed$ ssh merajahmed@10.237.22.140

##### merajahmed@vindhya:~$ jupyter notebook --no-browser --port=8889

##### Merajs-MacBook-Air:~ merajahmed$ ssh -N -f -L localhost:8888:localhost:8889 merajahmed@10.237.22.140


# SSH Login Without Password
#### Login to remote server without without password
<hr/>

##### Merajs-MacBook-Air:~ merajahmed$ ssh-keygen

##### merajahmed@vindhya:~$ ssh-copy-id -i ~/.ssh/id_rsa.pub merajahmed@10.237.22.140

