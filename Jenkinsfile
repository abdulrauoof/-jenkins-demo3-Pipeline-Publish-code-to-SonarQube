#!groovy
@Library('Sapient-DevOps@master') _
node{ 
 maven {
   MAVEN_BUILD_GOALS   = "clean install -e -X -Dmaven.test.skip=false"
   POM_FILE_PATH       = 'pom.xml'
   MAVEN_TEST_GOALS    = "test -e -X"
   SONAR_PROJECT_KEY   = 'kube-maven-sonarkey'
   SONAR_GOAL          = "sonar:sonar"
   SONAR_PROJECT       = 'SR Kube-Pipeline'
   mavenImageName      = 'maven:3.3.9-jdk-8-alpine'
   mavenImageTag       = 'latest'
   mavenContainerName  = 'maven'
   mavenWorkDir	       = '/home/jenkins'
   mavenClaimName      = "jenkins-pvc"

}
}

