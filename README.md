# CI/CD PIPELINE FOR SIMPLE JAVA APPLICATION.

The pipeline(Main pipeline) does that following steps

1. Checks out the from github repository.
2. Builds the Java code using Maven.
3. Does the static code analysis using Sonarqube.
4. Uploads the artifact to Nexus repository.
5. Deploys the artifact to tomcat server.


# Prerequisites required.

- Launch 4 EC2 instances and install Jenkins,Sonarqube,Nexus and Tomcat respectively.
- Make sure that the security group is configured with ports 9000(Sonarqube),8081(Nexus),Jenkins(8080),Tomcat(8080) in the inbound rules.
- Make sure all the services in the servers are up and running.
- Install Sonarqube Scanner agent in Jenkins and Configure Sonarqube URL in Jenkins, So that Static code analysis is done.
- Install Nexus Artifact uploader agent in Jenkins and Configure Nexus URL in Jenkins, So that Artifact can be uploaded in the Nexus Repository.
- Install SSH agent in Jenkins and Configure the key in Jenkins to Deploy the Artifact into Tomcat Server.


Once all the Prerequisites are completed , Pipeline Script can be executed in Jenkins by creating a PIPELINE project.





