# CI/CD PIPELINE FOR SIMPLE JAVA APPLICATION.

The pipeline(Main pipeline) does that following steps

1. Checks out the from github repository.
2. Builds the Java code using Maven.
3. Does the static code analysis using Sonarqube.
4. Uploads the artifact to Nexus repository.
5. Deploys the artifact to tomcat server.


# Prerequisites required.

1.Launch 4 EC2 instances and install Jenkins,Sonarqube,Nexus and Tomcat respectively.
2.Make sure that the security group is configured with ports 9000(Sonarqube),8081(Nexus),Jenkins(8080),Tomcat(8080) in the inbound rules.
3.Make sure all the services in the servers are up and running.
4.Install Sonarqube Scanner agent in Jenkins and Configure Sonarqube URL in Jenkins.
5.Install Nexus Artifact uploader agent in Jenkins Configure Nexus URL in Jenkins.
6.Install SSH agent in Jenkins and Configure the key in Jenkins.


All the Prerequisites are completed , Pipeline Script can be executed in Jenkins by creating a PIPELINE project.





