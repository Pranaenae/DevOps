# Complete Application Deployment Using Kubernetes Components

Create the Yaml file for mongo deployment.
![image](https://user-images.githubusercontent.com/80820244/236728711-35e91684-c13f-4e38-be65-c1d500915c7d.png)
 
 Create the Secret yaml file.
 ![image](https://user-images.githubusercontent.com/80820244/236731088-00e43722-31f3-41e5-b0e4-5a123ff21f8e.png)

Using an online encoder to base64 encode and decode.

![image](https://user-images.githubusercontent.com/80820244/236731127-69631343-4690-4ad9-904e-cefff8bf4983.png)

Create and view the secret.

![image](https://user-images.githubusercontent.com/80820244/236731689-7da33acc-1291-46f9-bf6e-ab213c2d1801.png)

Provide a reference to the secret file in the deployment file.

![image](https://user-images.githubusercontent.com/80820244/236731927-6eb33dba-3211-4e2b-8030-06670b64cc1f.png)

Create the deployment.

![image](https://user-images.githubusercontent.com/80820244/236732026-966ab888-693a-4d37-a5e9-42880bee5b68.png)

# Creating an internal service

Add service yaml to the file.

![image](https://user-images.githubusercontent.com/80820244/236732576-15ab1fef-1863-41a6-a0bd-df8845e93e55.png)

Apply the file.
![image](https://user-images.githubusercontent.com/80820244/236732887-6114590a-f1eb-4d97-8124-6ee102f03767.png)

Write yaml for mongo-express and service.
![image](https://user-images.githubusercontent.com/80820244/236733878-3c8f96e2-af22-48ff-958d-74307a3c09e7.png)
![image](https://user-images.githubusercontent.com/80820244/236733915-f6090302-b869-4021-b743-10f783d58e8b.png)

Write yaml for mongo-configmap.
![image](https://user-images.githubusercontent.com/80820244/236733791-dc36f1f1-ff9c-40eb-b563-688c5ada66c8.png)


Create the mongodb Configmap and mongo express deployment.

![image](https://user-images.githubusercontent.com/80820244/236733721-34b432f6-09de-4c4e-bc67-b87f0f3e3a15.png)

MongoDB external service created.

![image](https://user-images.githubusercontent.com/80820244/236734276-bb5af85e-0743-45d9-83d8-eecd4fa6abc8.png)
