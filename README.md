1. start 
sudo docker-compose -f docker-compose.yaml up -d
2. stop
sudo docker-compose -f docker-compose.yaml stop
3. stop & delete 
sudo docker-compose -f docker-compose.yaml down

4. 大保健
sudo docker-compose  --compatibility  -f docker-compose.yaml  up -d  --force-recreate

4. 登录taskmanager容器
sudo docker exec -it  tm-id  /bin/bash
 ./bin/flink run ./examples/streaming/WordCount.jar  --output worldcount.txt

 cat worldcount.txt


5. 内存调优
https://nightlies.apache.org/flink/flink-docs-master/zh/docs/deployment/memory/mem_setup/
