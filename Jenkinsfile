#!/usr/bin/env groovy

pipeline {
  agent any
  stages {
    stage('Static Analysis') {
      script {
        env['GIT_BRANCH'] = sh(
          script: "git branch | grep \* | cut -d ' ' -f2",
          returnStdout: true
        ).trim()
      }
      echo "The branch is ${GIT_BRANCH}"
    }
  }
}
    
