SonarQube installation on Ubuntu

#update server:
sudo apt update -y

#install OpenJDK:
sudo apt install openjdk-17-jre-headless

#Download and extract SonarQube:
sudo wget https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-9.4.0.54424.zip
sudo apt install unzip
sudo unzip sonarqube-9.4.0.54424.zip
sudo mv sonarqube-9.4.0.54424 sonarqube

#Add SonarQube user:
sudo adduser sonar
sudo chown sonar:sonar sonarqube-9.4.0.54424.zip -R

# change the permissions to the group user and other users:
sudo chmod 777 sonarqube -R

#switch to sonar user:
sudo su - sonar

#start the SonarQube:
cd /opt/SonarQube/bin/linux-x86-64
./sonar.sh start
./sonar.sh status

#sonarqube port no:9000
