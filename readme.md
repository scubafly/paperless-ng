#This setups paperless-ng on your synology NAS.

Original repo can be found here: https://github.com/jonaswinkler/paperless-ng

This will install jonaswinkler/paperless-ng:latest ( Tested with 1.1.0 )

##Installation

Template setup for paperless-ng

Enable SSH, login via putty (or other ssh client tool of your choice), execute sudo -i to become root and go to a new paperless folder.

Clone this repository.

Change folder mounts, ports, password, and username as you please and update the composer.yml file

Execute docker-compose up -d and wait for the main container to become healthy

After the all the containers are up and main container is healthy create the superuser account by executing this command:

docker-compose run --rm webserver createsuperuser

This will let you choose you superuser username and password. The password you can change later.

Original setup tutorial found here:
https://www.synoforum.com/threads/paperless-ng.5021/post-22562
