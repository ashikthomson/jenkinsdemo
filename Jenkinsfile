node{
   stage('SCM Checkout'){
   git 'https://github.com/ashikthomson/jenkinsdemo'
   }
   
   stage('Clean'){
   sh 'mvn clean'
   
   }
   stage('Install'){
   sh 'mvn build'
   
   }
}
