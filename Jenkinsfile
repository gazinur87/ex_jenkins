pipeline {
    agent 'master'

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
               sh 'cat Dockerfile'
            }
        }
    }
}
