sudo docker run -d  --name csvserver -p 9393:9300 infracloudio/csvserver:latest
sudo docker logs <container_id>
sudo docker cp inputdata csvserver:/csvserver/inputdata

sudo docker start <container_id>
