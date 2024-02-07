The necessary files are in the network folder. 

You'll need to run this on a linux system. For reference, I created the docker network on an ubuntu machine.

You'll need to run "sudo apt install docker docker.io docker-compose -y" to get the necessary tools. don't forget to apt update and upgrade beforehand.

after that, you'll cd into the assignment3 directory and run "sudo docker-compose up -d"

once the builds are complete, go to your broswer and type "https://localhost:443" to access dvwa through the https reverse proxy. This also connects
to a load balancer that uses Round-Robin to go through the two dvwa servers. You will find that logging in and mainting sessions will be a hassle using that connection method.

You can also go to localhost:8080 to access one of the dvwa containers through the modsecurity reverse proxy running on apache2.

have fun!

