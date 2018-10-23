Build Docker Images with Packer and Ansible

Read more
https://blog.james-carr.org/build-docker-images-with-packer-and-ansible-3f40b734ef4f

packer build ./packer_docker.json 

docker image import ./foo.tar demo:0.1

docker run -i -t demo:0.1 /bin/bash
root@93676e7c3381:/# ls /root/foo 
/root/foo
root@93676e7c3381:/# cat /root/foo 


