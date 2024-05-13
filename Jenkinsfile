pipeline {
  agent none
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/Souravte/fullstack-software', branch: 'main')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front-End Unit Test') {
          steps {
            sh 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}