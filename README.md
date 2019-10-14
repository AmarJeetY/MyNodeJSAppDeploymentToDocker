### MyNodeJSAppDeploymentToDocker
* Build , Test and Deploy simple Node.js application to docker as Image 
For this application to run successfully make sure that you heve created a rspoistry on Docker Hub  
Configure your credentials in your local jenkins installation as global credentails  
Updte ID of the global credentials in Jenkinsfile at below line  
In below case dockerhub is ID you must change with yours  
'https://registry.hub.docker.com', 'dockerhub'  
Also change name of the rspository with yours  
def app = docker.build("amarjeety/myrepository:${commit_id}", '.').push()
