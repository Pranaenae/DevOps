# Run an Nginx container and attach bash to it. 

Run the following code in terminal.

```
docker run -d -p 8081:80 --name webserver nginx
```
-d : detached mode
-p : port
8081 : host_port
80: container_port
name: local container name
nginx: image name in docker registry

![image](https://user-images.githubusercontent.com/80820244/236128672-1abbe4a2-07b7-4303-9080-9e38b50201a9.png)


Check the port in browser.
![image](https://user-images.githubusercontent.com/80820244/236128629-367c7f84-8ec0-4477-8b71-b8af584da563.png)

Attach bash to the created container.
```
docker container exec -it webserver bash
```

Test the bash.

![image](https://user-images.githubusercontent.com/80820244/236129358-4958b201-7429-45ce-bd9c-57ef665946b4.png)


Stop the container and remove it from memory.

![image](https://user-images.githubusercontent.com/80820244/236130152-c11b7111-4503-415f-a21e-5ac87f9d08d0.png)


Delete the downloaded image.

![image](https://user-images.githubusercontent.com/80820244/236130419-19f31154-b715-4d97-bdee-5c24850e3497.png)
