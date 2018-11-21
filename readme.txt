I have created two instance and renamed hostname to MSR-test-Instance-1 & MSR-test-Instance-2
steps to rename 
     sudo vi /etc/hostname
          MSR-test-Instance-1

     sudo vi /etc/hosts
         127.0.1.1 MSR-test-Instance-1
         
     systemctl restart systemd-logind.service
     hostnamectl set-hostname MSR-test-Instance-1
     
I have installed configuration management tool ansible in instance and written a yaml code to install below packeges and I have attached my yaml code in it
   ● NVM – Version 0.33.2
   ● Node – 8.12.0
   ● Docker – 18.06 or latest
   ● Docker Compose – 1.13 or latest
   ● Openssl – latest version
   ● Git – latest version
I have created a apache web-server container in MSR-test-Instance-1 using Docker Compose file and cross checked it in port 8040 and i have created yaml file to install apche web-server in docker container and i have attached yaml file and docker-compose file in it.
I have created a couchDB container in MSR-test-Instance-2 using Docker Compose file and cross checked it in port 8080 and i have created yaml file to install couchDB in docker container and i have attached yaml file docker-compose file in it.
I have added all the yaml file in my git repository
