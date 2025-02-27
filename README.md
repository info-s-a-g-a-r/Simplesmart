Cloud Infrastructure Trainee (Assignment)

Step1: Using AWS Cloud, Launched 2 VMs 
        a.Master
        b.Slave
Step2: Installed & Configured Docker, Kubernetes on both VMs
Step3: On Master Node Created a new directory ( my-web)
        inside the directory create app.js, package.json, Dockerfile

   1. app.js
      # This file contains the core logic of the application
      # app.js sets up a simple HTTP server that returns "Hello, World!" when accessed.

  2. package.json
     # This file is the manifest for your Node.jsproject. It includes metadata about your application, such as its name, version, and dependencies

  3. Dockerfile
     # The Dockerfile defines the instructions for building a Docker image of your application.

Step4: To  Build  Docker Image 
       # docker build -t my-web .
       To Run The Container 
       # docker run -p 3000:3000 my-web
To Verify/Access the application Copy The Public IP of Master and Paste in the browser with port number 3000
      <PublicIP:3000>

Step5: Create Deployment.yaml  &  Service.yaml files 
      Deployment and Service YAML files are crucial components in Kubernetes that enable you to define and manage your application's lifecycle and how it is accessed

  To apply deployment.yaml  & service.yaml use the cmd:
  #kubectl apply -f deployment.yaml
  #kubectl apply -f service.yaml

  To access / verify  the application  copy the public IP of master and nodePort:30002(specified) you'll see 'Hello World"
  <publicIP:30002>


      
  
 
