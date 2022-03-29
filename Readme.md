# Base docker image

Base image to supply docker image which shares data between host and guest.
Host uses data folder (empty inside this repo) and is mapped to guest user homeidr: /home/myuser
entrypoint.sh script makes sure the owner rights of guest are mapped to user id of host to avoid issues there

# Start
```docker-compose run baseimage /bin/bash```