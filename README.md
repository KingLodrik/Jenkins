# Jenkins


How to install jenkins on ubuntu
  
  update:
    1) sudo apt-get update 
  
  Add open repo and install java:
    2) sudo add-apt-repository universe
    3) sudo apt install openjdk-8-jre-headless
  
  Installation:
    4) wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
    5) sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
    6) sudo apt-get update
    7) sudo apt-get install jenkins
    
  Cheking jenkins work or not:
    8) ps -ef | grep jenkins
    9) service jenkions status 
    10) sudo service jenkins start/ stop

    
 How to run with war-file and tomcat9
    
  Install war-file:
    11) cd
    12) wget http://mirrors.jenkins.io/war-stable/latest/jenkins.war
  
  Deploy java to war-file:
    13) java -version
    14) which java (to find locatin of java )
    15) /user/bin/java -jar jenkins.war
            * now you can creat your jenkins with 8080 port
    16) ctrl + c ( to stop runing jenkins with war file )
    
 Install tomcat9
    17) wget https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.0.M10/bin/apache-tomcat-9.0.0.M10.tar.gz
    18) tar xzf apache-tomcat-9.0.0.M10.tar.gz
    19) mv apache-tomcat-9.0.0.M10 tomcat9  (you have install tomcat)
 
 Deploy tomcat to war file:
    20) cd tomcat/ then ls
    21) cd webapps/ then ls
    22) cp jenkins.war tomcat9/webapps/ ( have deploy war file to webapps )
    23) cd bin
    22) ./startup.sh
    
    
 refe: (1)  https://hostadvice.com/how-to/how-to-install-jenkins-automation-server-on-ubuntu-18-04/
       (2)  https://www.edureka.co/blog/install-jenkins/
    
  
    
   

 


   
 
