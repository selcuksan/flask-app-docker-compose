pipeline {
  agent any
  stages {
    stage("build") {
      steps {
          sh 'echo "build stage"'
      }
    }
    stage('test') {
      steps {
         sh 'echo "test stage"'
      }
    }
    stage('deploy') {
      steps {
         sh 'echo "deploy stage"'
      }
    }
  }
}
