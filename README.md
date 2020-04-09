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


# Set hostname to server IP on local computer 
<hr/>

##### Merajs-MacBook-Air:~ merajahmed$ sudo vi /etc/hosts
##### Add entry after last line ip_addr {tab} name and save


# Access IITD internal website from home
<hr/>

##### 1) ssh -D 1234 <usename>@sri.cse.iitd.ac.in
  
#### 2) fir apne browser ke proxy mei jke set socks5 proxy to localhost:1234

#### 3) And enable proxy dns over socks5

#### Now internal website can be accessed from browser

##### Note: Revert the settings after work done
##### Credit: Prateek
  
