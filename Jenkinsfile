pipeline {
  agent none
  stages {
    stage('Checkout Code') {
      steps {
        sh 'ls -la'
        git(url: 'https://github.com/Souravte/fullstack-software', branch: 'main')
      }
    }

  }
}