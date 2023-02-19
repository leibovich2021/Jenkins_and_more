Jenkins
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


**********************
-----------------------------------------------------------

**********************

Jenkins Deploy from GitHub

plug to Download:
Git plug

jenkins->Login to GitHub->git clone->Build/compile->Test->Deploy->WebServer(AWS)

we need:
1.repository
2.jenkins job
3.key from computer ( ssh-keygen)
public key go to github and praivte key go to jenkins



1. Create a new repository in GitHub
push to github some file.
2.in Jenkins job go to Configuration -> Genetal -> GitHub project, and put our url link from GitHub repository
3.in Jenkins job go to Configuration -> Source Code -> Git-> Repositories  
4. create Credentials of server (dont forghet ssh key to git from computer)
Dashboard->Manage Jenkins->Configure Global Security-> Git Host Key Verification Configuration 
change to  Host Key Verification Strategy=Accept first connection
5. to deploy in server we  Send build artifacts over SSH

**********************
-----------------------------------------------------------

**********************

Build Job from GitHub -   Jenkins Build Triggers (webhook)
GitHub hook trigger for GITScm polling


Dashboard->test-job->Configuration->General->GitHub project
Project url + GitHub hook trigger for GITScm polling\

now in github go to Webhooks
http://13.40.192.241:8080/github-webhook/




**********************
-----------------------------------------------------------

**********************

Jenkins Pipeline and Jenkinsfile

plug to Download:
pipeline

to open permission denied
sudo chmod 666 /var/run/docker.sock



