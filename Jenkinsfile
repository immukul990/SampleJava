pipeline {
  agent any
  stages {
    stage('GetCode'){
            steps{
                git 'https://github.com/immukul990/SampleJava.git'
            }
         }
    stage ('Build') {
      steps {
        sh 'echo Hello Build stage'
      }
    }
    stage ('Test') {
      steps {
        sh 'echo hello Test stage'
      }
    }
    stage('SonarQube analysis') {
//    def scannerHome = tool 'SonarScanner 4.0';
        steps{
        withSonarQubeEnv('sonarqube-8.9') { 
    }
        }
        }
       
  }
}
