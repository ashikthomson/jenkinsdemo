node{
   def mvnHome
   stage('Preparation'){
       git 'https://github.com/ashikthomson/jenkinsdemo.git'
       mvnHome = tool 'maven3'
    }
   stage('Build'){
      withEnv(['%MAVEN_HOME%=$mvnHome']){
           bat(/"%MAVEN_HOME%\bin\mvn" -Dmaven.test.failure.ignore clean package 
pause/)
      }
   }
}