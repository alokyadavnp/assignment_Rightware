# assignment_Rightware

# BUILD with Vagrant File
# configured service is SSH for remote connection to the docker container

1. go into the Vagrant root directory and run the command,
        "vagrant up" or "vagrant reload"
        
   ![Screenshot from 2022-03-04 10-48-43](https://user-images.githubusercontent.com/61194564/156735272-8d307bec-f9ce-48ac-9725-fcd0fec9befd.png)
   
2. To check into the running status of the Docker run the command
         "Docker ps"
         
   ![Screenshot from 2022-03-04 11-10-20](https://user-images.githubusercontent.com/61194564/156735435-d0c90700-021e-4799-94b8-47bb58c8f236.png)
 
3. We can ssh to the running container using command in other terminal
         ssh test@<ip_to_the_container> -p 220 --> do check for the port, if it is already in use change port to something else from Vagrantfile and password to the server is set to be "test" for testing purpose and port 220 of virtual machine with container port of 22)
         
   ![Screenshot from 2022-03-03 14-23-16](https://user-images.githubusercontent.com/61194564/156735158-d299dc36-5354-4284-89da-ac073c785069.png)
         

      


# Deploy with Ansible

# Deployed here is a react webapp. This web application takes down your note and pins on the screen.

1. Go into the application root directory
2. Run the command, 
       "ansible-playbook build.yml"
3. Ansible is deployed in the localhost and on port 3000, use the address "localhost:3000" to access the webapp.

![Screenshot from 2022-03-04 11-22-23](https://user-images.githubusercontent.com/61194564/156736007-51fccd5b-dd41-4bdb-8ef5-8d7381e54681.png)


