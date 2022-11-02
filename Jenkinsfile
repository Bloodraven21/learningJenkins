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

    stage('dockerBuild') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile .'
      }
    }

  }
}