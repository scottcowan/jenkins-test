#!/usr/bin/env groovy

pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        echo 'scm : the commit branch  is ' + env.BRANCH_NAME
      }
    }
    stage('Build') {
      steps {
        echo 'Pulling...' + env.BRANCH_NAME
        checkout scm       
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
    
