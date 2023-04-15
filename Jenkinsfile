pipeline {
    agent {
        label 'slave-ubuntu'
    }
    stages {
        stage("build"){
            steps{
                echo "building the application"
            }
        }
        stage("test"){
            steps{
                echo "testing the application"
            }
        }
        stage("deploy"){
            steps{
                echo "deploying the application"
                sh 'docker-compose up'
            }
        }
    }
}
