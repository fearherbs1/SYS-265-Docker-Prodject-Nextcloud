# Requirments:
Ubuntu Server 20.3 with docker and docker-compose installed  
You can follow my guide [HERE](https://github.com/fearherbs1/SYS-265-02-Tech-Journal/wiki/Docker-Lab) if you need asistance. 

# Useage:
clone this repo into your desired folder:

`git clone https://github.com/fearherbs1/SYS-265-Docker-Prodject-Nextcloud.git`  

Edit the mariadb database username and password to your liking in docker-compose.yml:

```
      - MYSQL_ROOT_PASSWORD=rootpassword
      - TZ=America/New_York
      - MYSQL_DATABASE=nextcloud
      - MYSQL_USER=nextcloud 
      - MYSQL_PASSWORD=nextcloudpassword 
      - REMOTE_SQL=http://URL1/your.sql,https://URL2/your.sql 
```

Start the containers with:  
`sudo docker-compose up -d`  

Once started, navigate to https://(yourserverip) and you should see the nextcould startup page:  
