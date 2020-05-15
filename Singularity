Bootstrap: docker
From: centos:8

%runscript
    exec echo "The runscript is the containers default runtime command!"


#%files
#   /home/vanessa/Desktop/hello-kitty.txt        # copied to root of container
#   /home/vanessa/Desktop/party_dinosaur.gif     /opt/the-party-dino.gif #

%environment
    VARIABLE=MEATBALLVALUE
    export VARIABLE


%labels
   AUTHOR simone.roz@gmail.com

%post
    apt-get update && apt-get -y install python3 git wget
    mkdir /data
    echo "The post section is where you can install, and configure your container."
