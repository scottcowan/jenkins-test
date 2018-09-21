#!/usr/bin/env groovy

pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        echo 'scm : the commit branch  is ${BUILD_BRANCH}'
      }
    }
    stage('Build') {
      steps {
        
        echo "Building..."
      }
    }
    stage('Test'){
      steps {
        echo "Testing..."
      }
    }
    stage('Deploy Mock'){
      steps {
        echo "Deploy Mock..."
      }
    }
    
  }
}
    
