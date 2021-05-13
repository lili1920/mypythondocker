
1. mkdir /tmp/test

2. sudo docker build -t directory-monitor .

3.sudo docker run -d --restart=always -e DIRECTORY='/tmp/test' -v /tmp/:/tmp/ directory-monitor

4- touch /tmp/test/example.txt

5- sudo docker logs CONTAINER_ID
