#!/usr/bin/env groovy

pipeline {
  agent any
  stages {
    stage('Get Artifacts') {
      steps {
        echo 'scm : the commit branch  is ' + env.BRANCH_NAME
      }
    }
    stage('Mock'){
      steps {
        echo "Deploy to mocked environment..."
      }
    }
    stage('Integration') {
      when {
          expression { env.BRANCH_NAME == 'master' }
      }
      steps {
          echo "Deploying to Integration"
      }      
    }
    stage('Prod') {
      when {
          expression { env.BRANCH_NAME == 'master' }
      }
      steps {
          echo "Deploying to Production"
      }      
    }    
  }
}
    
