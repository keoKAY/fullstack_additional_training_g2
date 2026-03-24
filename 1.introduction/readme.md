## NOTE 
- prepare environment for testing and learningg about linux machine 


+ **Requirements** 
- vagrant 
- oracle virtualbox 
```bash 
cd 1.introduction
vagrant init ubuntu/jammy64
# edit the cofiguration file 
vagrant up 
vagrant status 
# in order to access your machine via SSH 
vagrant ssh 


# if you uupdate the config, want to apply to you machine 
vagrant reload 
vagrant halt # to shutdown 
vagrant destroy -f  # to delete the machine 

```