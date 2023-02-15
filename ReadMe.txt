
**********************

Jenkins -> Build/Commpile -> Test -> Deploy -> AWS(WebServer)

Open Server in AWS(EC2)
Open new item in Jenkins

to Executr shell put cat index.html

For SSH We need:
1. plug to Download:
Publish Over SSH 
2.Open in Job -> Publish Over SSH -> Post-build Actions ->  Send build artifacts over SSH
3.Open in Dashboard -> Manage Jenkins -> Configure System ->  Publish over SSH 
(we need oped access sudo chmod 777 -R /var/www/html/)

**********************
-----------------------------------------------------------

**********************

Jenkins Slaves/Nodes
open server in aws of ubuntu system

plug to Download:
SSH Slave
SSH Agent

**install java**
go to :    Dashboard -> Manage Jenkins -> Nodes -> New Node
Create new Node(=slave) (launch method via SSH). and Create Credentials

*Labels*



