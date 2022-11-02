pipeline {
  agent any
  stages {
    stage('CheckoutCode') {
      parallel {
        stage('CheckoutCode') {
          steps {
            git(url: 'https://github.com/Bloodraven21/learningJenkins', branch: 'master')
          }
        }

        stage('logs') {
          steps {
            sh 'ls -la'
          }
        }

      }
    }

  }
}