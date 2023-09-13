pipeline {
  agent any
  stages {
    stage("verify tooling") {
      steps {
        sh '''
          docker version
          docker info
          docker-compose version 
        '''
      }
    }
    stage('Start container') {
      steps {
        sh 'docker-compose up -d --no-color --wait'
        sh 'docker-compose ps'
      }
    }
  }
  post {
    always {
      sh 'docker-compose ps'
    }
  }
}
