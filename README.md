# Hommme
1.  apt list ngnix
    sudo su
    apt install ngnix
    y
    apt remove ngnix 
    apt autoremove
    y
2. sudo su
   cd /etc/apt/sources.list.d/
   cat > vb.list 
   deb [arch=amd64 signed-by=/usr/share/keyrings/oracle-virtualbox-2016.gpg] https://download.virtualbox.org/virtualbox/debian <mydist> contrib
   nano vb.list
   deb [arch=amd64 signed-by=/usr/share/keyrings/oracle-virtualbox-2016.gpg] https://download.virtualbox.org/virtualbox/debian jammy1 contrib
   wget -O- https://www.virtualbox.org/download/oracle_vbox_2016.asc | sudo gpg --yes --output /usr/share/keyrings/oracle-virtualbox-2016.gpg --dearmor
   sudo apt update
   sudo apt install virtualbox-7.1
   y
