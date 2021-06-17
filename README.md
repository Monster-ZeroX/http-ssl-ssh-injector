# http-ssl-ssh-tunneling
http ssl ssh tunneling vpn for android and linux devices

# packages :

[+] - apt install -y git python openssh sshpass netcat-openbsd corkscrew screen

[+] - badvpn-tun2socks must be compiled and installed https://github.com/ambrop72/badvpn

[+] - in proxification.sh line 6  "sudo route add $ssh_ip gw 192.168.43.1 metric 5" 192.168.43.1 must be replaced with your default gateway

[+] - on arch and some other linux distros netcat-openbsd is called openbsd-netcat

[+] - apt install screen 

# configuration :

past your data into file settings.ini 

![image](https://user-images.githubusercontent.com/46646744/121788894-356af880-cbc9-11eb-81b6-856675bad994.png)

note : if are using Direct ssh leave the first part of settings.ini file empty you have only to setup your ssh settings

note 2 : if not woks in defaul auto_replace value , update it to auto_replace = 1 in file settings.ini

![image](https://user-images.githubusercontent.com/46646744/121788947-9bf01680-cbc9-11eb-8b84-4682f58d1387.png)


# how it works!

(root is required in android )

[+] - git clone https://github.com/abdoxfox/http-ssl-ssh-injector.git

# if you will use custom payload or direct ssh connection :

* setup yor custom payload and proxy (if need it  else leave it empty) and ssh details in settings.ini file.

[+] - cd http-ssl-ssh-injector

[+] - sudo  or tsu for termux  #run as root

[+] - chmod +x runvpn.sh

[+] - ./runvpn.sh 1          (argument 1 means that you will use payload / direct ssh connection)

 # if are using ssl (sni bughost )

* setup your sni bughost and ssh details in settings.ini file and run the following commands :

[+] - cd http-ssl-ssh-injector

[+] - sudo or tsu 

[+] - chmod +x runvpn.sh

[+] - ./runvpn.sh 2         (argument 2 means that you will use ssl  method )


# screenshots 

![image](https://user-images.githubusercontent.com/46646744/121225010-00853b80-c881-11eb-8cb6-4fcea95f8f88.png)

* note : to stop the script press CTRL + C

![image](https://user-images.githubusercontent.com/46646744/121225175-2c082600-c881-11eb-9c82-27fc2f4200a1.png)


screenshots from : @megasniff_v2 (thanks a lot bro)


