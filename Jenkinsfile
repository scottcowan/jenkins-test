#!/usr/bin/env groovy

pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        script{
          env['GIT_BRANCH'] = sh(
              script: "git branch | grep \\* | cut -d ' ' -f2",
              returnStdout: true
          ).trim()
        }
        echo 'scm : the commit branch  is ' + env.GIT_BRANCH
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
    
