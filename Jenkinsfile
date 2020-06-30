pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building.. ${env.build_id}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
               sh 'cat Dockerfile ${env.build_id}'
            }
        }
    }
}
