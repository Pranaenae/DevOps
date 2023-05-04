# Storing Data Outside a Container

Create a volume.

![image](https://user-images.githubusercontent.com/80820244/236171846-4c03b8a7-35a8-4adf-981b-99cb27feb4ef.png)

Run an nginx container that uses the volume.
```
docker run -d --name voltest -v myvol:/app nginx:latest
```

-d detached 
--name voltest = Instance name
-v myvol:/app nginx:latest = Map created myvol to /app folder in nginx image

![image](https://user-images.githubusercontent.com/80820244/236173365-e5b29c41-c926-404f-aa2e-d29fb64c4b78.png)

Attach bash to the created instance.
```
docker exec -it voltest bash
```

![image](https://user-images.githubusercontent.com/80820244/236173640-41a3c66f-03c0-4646-b48c-93b4dfdff8b3.png)


Install nano in the container

```
apt-get update
apt-get install nano
```
![image](https://user-images.githubusercontent.com/80820244/236174026-3b963e94-ee7b-490f-a5e9-b8fe39f48407.png)

## Add a file using nano.

```
cd app
nano test.txt
```

Save using ctrl+o ctrl+x.

![image](https://user-images.githubusercontent.com/80820244/236174347-40b6483d-dffc-4550-8ea0-e8a31f40f093.png)

![image](https://user-images.githubusercontent.com/80820244/236174697-41afcb74-8c63-403d-b102-f100fe72808c.png)


Stop the container instance.

![image](https://user-images.githubusercontent.com/80820244/236175072-54e9d119-418e-40e1-8cca-d25f72232dc4.png)

Remove the container.

![image](https://user-images.githubusercontent.com/80820244/236175144-ead2767c-7c2f-4152-a22f-09e33568ad9b.png)

Use the same commands to create a new volume. Check if test.txt still exists.

![image](https://user-images.githubusercontent.com/80820244/236175407-6f0ed1ef-ceff-42b4-a6ec-02afcf06349c.png)

