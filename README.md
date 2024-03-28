# Cloned-jira-server-setup
set up cloned server to UAT test env

stop jira

aws --> network team can give cloneed server for us

1.if we have cloned server first we need to see 

check 2 things db.config file and server.xml file

2. in this we have all jira software is installed and database is installed , we just need to update some of the things in db.config file and server.xml file

we have our cloned server in diffrent ip adresss

3. go to intalation directory
    
opt/

4.in server.xml 

we have proxy url:

in https/http we have port also

for https:443

http: jira:8080 confluenc:8090

in connector port :proxyname, proxyport,etc 

we can difrenciate cloned server by IP adress

<remove scheme, proxyname,proxy port in the connector port>

we can access jira through IP adress 

5. in Db config file

when cloned the prod db and cloned dp is point towords same , so we need to change

var/atliasn/application-data/

check db.config file 


dpurl end point--> host:<IP adresss/> or localhost

6. /opt/atlassian/bin/ .start.jira

we can use prod licence key for UAT also

use ipadress:port<8080> in chrome

7. change base url 


