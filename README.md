# Docker_task

This is a website focused on providing the best of the content needed by a Computer Science Engineering student at one location. <br/>
I created it using HTML-Bootstrap-JQuery alongwith min.js that comes along with Bootstrap. This website has been deployed on Docker container running on my RHEL8 machine. Alongwith that I also deployed it on AWS EC2 instance.<br/>
I used a HTTPD image to start a webserver on port 8085 of my host machine using port forwarding of port 80 of httpd image to make it available to outside world. <br/>
Also to make it public I used "NGROK" software which made this website available to a public network. <br/>

Commands used:

1 - docker pull httpd <br/>
2 - mkdir docker_storage <br/>
3 - cd docker_storage/ <br/>
4 - git clone <repository-ip> <br/>
5 - docker run -dit --name webserver -v docker_storage/:/usr/local/apache2/htdocs/ -p 8085:80 httpd:latest <br/>

I would like to say thanks to Vimal Daga sir from linuxworld for teaching me such a wonderful technology and providing the opportunity to be  a part of this great initiative IIEC Rise.
