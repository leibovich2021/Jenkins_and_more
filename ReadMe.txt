jenkins




**********************
Jenkins -> Build/Commpile -> Test -> Deploy -> AWS(WebServer)

plug to Download:
Publish Over SSH 

Open Server in AWS(EC2)
Open new item in Jenkins

to Executr shell put cat index.html


Publish Over SSH -> Post-build Actions ->  Send build artifacts over SSH
Dashboard -> Manage Jenkins -> Configure System ->  Publish over SSH 
(we need oped access sudo chmod 777 -R /var/www/html/)


**********************
