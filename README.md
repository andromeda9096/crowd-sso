## Atlassian crowd-sso full on docker

### bash
```
docker volume create --name crowdVolume

docker run -v crowdVolume:/var/atlassian/application-data/crowd --name="crowd" --restart unless-stopped -d -p 6095:8095 andromeda9096/crowd-sso:0.0.2
```
### open in browser for firt config

http://hostip:6095  => jdbc:mysql://database-ip:port/crowd
