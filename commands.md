show config system login
show cli authorization 

show interafces

show route 


## making a user and giving them ssh access using password

set system login user kiprop class super-user
set system login user kiptop authentication plain-text-password 
set system services ssh 
commmit
exit


## make a user and let them login using ssh key 

set system login user kiprop class super-user
set system login user kiprop authentication ssh-rsa 'the key to login @kiprop'

## checking config

run show configuration 
