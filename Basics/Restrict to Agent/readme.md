# Restrict job to agent

Errors encountered: All nodes offline. Fix: Create the jenkins directory in home directory.

Go to configure clouds and enter the docker host URI and enable it.
![image](https://user-images.githubusercontent.com/80820244/236088971-1d5e371d-a9bb-41f4-bb1b-2bcdd7e372b5.png)

Create the docker agent template.

![image](https://user-images.githubusercontent.com/80820244/236089061-8a7a1c63-b90b-471b-bac3-0f619c535c3e.png)

Configure the job to be restricted to the created agent.

![image](https://user-images.githubusercontent.com/80820244/236089161-90960ed5-f55c-487b-81cd-3ca811dc9067.png)

Build the job.

![image](https://user-images.githubusercontent.com/80820244/236092477-2e4869d2-7847-4bbb-bb8b-dd25ba5e0ade.png)

## For python job
Load a new docker image with python3 support.

![image](https://user-images.githubusercontent.com/80820244/236093036-279d1d9e-742c-4df8-b0ff-13712784e51d.png)

We can see the build running in the specified agent. ![image](https://user-images.githubusercontent.com/80820244/236093379-1cc2c531-d029-4642-8f9b-62312ea852f4.png)

Build run successfully.

![image](https://user-images.githubusercontent.com/80820244/236093675-cbca79df-5a76-4260-97ac-a3271a5e9148.png)
