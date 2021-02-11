Template setup for paperless-ng

Change folder mounts, ports, password, and username.

Make mount folders on synology nas

ssh to synology nas

Make the folder on your Synology SmartHome/paperless and copy the .yml and .env files to it.

Enable SSH, login via putty (or other ssh client tool of your choice), execute sudo -i to become root and go to docker/paperless-ng folder.

Execute docker-compose up -d and wait for the main container to become healthy

After the all the containers are up and main container is healthy create the superuser account by executing this command:

docker-compose run --rm webserver createsuperuser

This will let you choose you superuser username and password. The password you can change later.

Original setup tutorial found here:
https://www.synoforum.com/threads/paperless-ng.5021/post-22562
