pipeline {
  agent none
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/Souravte/fullstack-software', branch: 'main')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile . -t souravdevops123/front-end'
      }
    }

  }
}