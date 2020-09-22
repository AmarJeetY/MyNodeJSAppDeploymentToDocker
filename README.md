### MyNodeJSAppDeploymentToDockerHub
* Build , Test and Deploy simple Node.js application to docker repository.  
1. For this application to run successfully make sure that you have created a rspoistry on Docker Hub  
2. Configure your credentials in your local jenkins installation as global credentials  
3. Updte ID of the global credentials in Jenkinsfile  
4. In below case replace dockerhub with yours  
````csharp  
'https://registry.hub.docker.com', 'dockerhub'  
````   
5. Change name of the repository with yours  

````csharp  
def app = docker.build("amarjeety/myrepository:${commit_id}", '.').push()
````  
