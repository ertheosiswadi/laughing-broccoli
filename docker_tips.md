#### Start Container
```
cd ~/Projects/ccle
sudo -E bin/moodle-docker-compose up -d
```
#### Stop Container
```
cd ~/Projects/ccle
sudo -E bin/moodle-docker-compose stop
```
#### SSH into Container
`sudo docker exec -it moodledocker_webserver_1 bash`
