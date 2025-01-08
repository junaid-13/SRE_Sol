**Step 1**

sudo docker run -d  --name csvserver -p 9393:9300 infracloudio/csvserver:latest
sudo docker logs <container_id>
sudo docker cp inputdata csvserver:/csvserver/inputdata

sudo docker start <container_id>


**In Step 2 again i had run this commands**


#Replace the {directory with the directory in which the inputdata file is present
sudo docker cp {directory}/inputdata csvserver:/csvserver/inputdata

**In Step 3 also you need to run the below mentioned command to start the csvserver without the error as inputdata not found**
sudo docker cp {directory}/inputdata csvserver:/csvserver/inputdata
