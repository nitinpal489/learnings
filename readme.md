fisrtly, writing the dockerfile by taking the ubuntu as the base image.
inside that, installing the apt-get package, updating that with the lastest version.
taking the zip file from browser to have the overall website link with in .zip extension based file.
while defining the .zip inside the ADD command bcz add command here will add the linking file, unzip the file to target destination. however we have already defined the specified path for the destination.
now, copy command will does the automation here like it will just copy the /tmp file inside the /var/www/html location.
in another command we just specified the port 80 fo our OS.
here, we defined that apache will be running in detached mode with the foreground basis.
-----------------------------------------------------------------------------------------

here, comes the command line.
open the gitbash, fetch the command ssh -i ......
sudo su-
yum install docker -y
systemctl start docker
systemctl enable docker
mkdir file1
cd file1
go inside the file1
case 1: 
vi Dockerfile
whatever the code is present in dockerfile, you can define the code here.
or
case 2:-
wget http://zzzzzzzzzzzzzz.zip /tmp
unzip the above file.
remove the .zip and stay with html file
now duilf the image.
docker build -t myimg .
docker images
docker run -d -p 3100:80 myimg 
(see the conatier list with port number).
assign the security group with the 3100 as for everywhere.

take the publicip:3100
run your website

now, fetching the image with tag assigned to dockerhub.
1. use dockerhub credentials to login using the command docker login
give username and password.
2. after that assign the tag to the images.
use docker push command to push the image to dockerhub.
3. after pushing check the dcokerhub inside the repository, whether it created or not.

=======================================================