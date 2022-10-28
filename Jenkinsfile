pipeline {
  agent any
  stages {
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
        steps{
        withSonarQubeEnv('sonarqube-8.9.1') { 
    }
        }
        }
       
  }
}
