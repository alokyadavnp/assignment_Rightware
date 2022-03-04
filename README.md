# assignment_Rightware

# BUILD with Vagrant File
# configured service is SSH for remote connection to the docker container
# Dockerfile contains command used in Ubuntu so recommended to use same.
1. go into the Vagrant root directory and run the command,
        "vagrant up" or 
        "vagrant reload"
2. To check into the running status of the Docker run the command
         Docker ps
3. We can ssh to the running container using command in other terminal
         ssh test@<ip_to_the_container> -p 220 --> do check for the port, if it is already in use change port to something else from Vagrantfile and password to the server is set to be "test" for testing purpose and port 220 of virtual machine with container port of 22)


# Deploy with Ansible

# Deployed here is a react webapp. This web application takes down your note and pins on the screen.

1. Go into the application root directory
2. Run the command, 
       "ansible-playbook build.yml"
3. Ansible is deployed in the localhost and on port 3000, use the address "localhost:3000" to access the webapp.

