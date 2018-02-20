#!groovy

pipeline {
  agent none
  stages {
    stage('Maven Install') {
      agent {
        docker {
          image 'Oracle BPM Quickstart 12.2.1'
        }
      }
      steps {
        sh 'mvn clean install'
      }
    } 
  }
}