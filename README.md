# Jenkins


How to install jenkins on ubuntu
  
  update:
    1) sudo apt-get update 
  
  Add open repo and install java:
    2) sudo add-apt-repository universe
    3) sudo apt install openjdk-8-jre-headless
  
  Installation:
    4) wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add - 
    5) sudo sh -c 'echo deb https://pkg.jenkins.io/debian binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
    6) sudo apt-get install jenkins
    
  Cheking jenkins work or not:
    7) ps -ef | grep jenkins
    8) service jenkions status 
    9) sudo service jenkins start/ stop

    
 How to run with war-file and tomcat9
    
  Install war-file:
    10) cd
    11) wget http://updates.jenkins-ci.org/download/war/2.7.3/jenkins.war
    12) 


   
 
