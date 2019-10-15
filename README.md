### MyNodeJSAppDeploymentToDocker
* Build , Test and Deploy simple Node.js application to docker as Image  
1. For this application to run successfully make sure that you heve created a rspoistry on Docker Hub  
2. Configure your credentials in your local jenkins installation as global credentails  
3. Updte ID of the global credentials in Jenkinsfile  
4. In below case dockerhub is ID you must change with yours  
````csharp  
'https://registry.hub.docker.com', 'dockerhub'  
````   
5. Also change name of the repository with yours  

````csharp  
def app = docker.build("amarjeety/myrepository:${commit_id}", '.').push()
````  
