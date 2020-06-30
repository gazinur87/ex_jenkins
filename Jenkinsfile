pipeline {
    agent any
    environment {
        // Using returnStdout
        CC = """${sh(
                returnStdout: true,
                script: 'echo "clang"'
            )}""" 
        // Using returnStatus
        EXIT_STATUS = """${sh(
                returnStatus: true,
                script: 'exit 1'
            )}"""
    }
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
        stage('print') {
            steps {
               sh 'printenv'
            }
        }
    }
}
