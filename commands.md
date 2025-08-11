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




show interfecare terse - ip or just if up or down 
show interfaces brief 
show interafaces 
show interface detail
show interface extensive


show interfaces terse xe-0/1/1

cli is hieractical 

physical interafaces can be divied more logical units 

valna tags - > just to say the vlan it belongs to 

all subnets in one interfaces. having more 


admin - > if someone has done it 
link -> if its down , up for one or both 

show interfaces bried xe-/1/1/*  -> all that started 


show interdfaces descrption

deploy with desciprtions , then when someone comeones they can know the use of the interface.
how do I check speed ?  - show interface xe-1/0/0 media
how do I check if an interface flapped? -> show interface detail

shoe interaces ge*


summary want to know about interafces in junos -> show intercaes , you can choose to be brief, terse, detail or extensive.



show interafces can also show -> current address , you can modify the address which will show in the current address nd have the mac adress ., when it last flapeed upto like 1 week 9 days.



couunt, match find execpt 
show interfaces terse xe-1/0/* | match down

show interaces terse xe-0/1/0 | 

show interfaces terse | match "physical|donw"

you can use mutiple pipes to filter more than once, its like having an hierachy.

myou can like match the physcical then count 

if you want to start at the firts  use find 







summary - > show interfaces commadd can tell you al ot- when it flapped, the speed and so much more. you can filter the output to just get what you need using macth, execept and others with a pipe apassing the output of original command to it.

