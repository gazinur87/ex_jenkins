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
                sh "echo ${env.build_id}"
            }
        }
        stage('Deploy') {
            steps {
               sh 'cat Dockerfile'
            }
        }
    }
}
