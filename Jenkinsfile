pipeline {
    agent {
        dockerd { image 'busybox' }
    }
    //   parameters {
    //     string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    // }
    // environment {
    //     // Using returnStdout
    //     CC = """${sh(
    //             returnStdout: true,
    //             script: 'echo "clang"'
    //         )}""" 
    //     // Using returnStatus
    //     EXIT_STATUS = """${sh(
    //             returnStatus: true,
    //             script: 'exit 1'
    //         )}"""
    // }
    stages {
        stage('test docker') {
            steps {
            sh 'whoami'
            }
        }

        // stage('Build') {
        //     steps {
        //     sh 'asd || true'
        //     sh "echo ${currentBuild.result}"
        //     }
        // }
        // stage('Test') {
        //     steps {
        //         sh "echo ${currentBuild.result}"
        //     }
        // }
        // stage('Deploy') {
        //     steps {
        //        sh 'cat Dockerfile'
        //     }
        // }
        // stage('print') {
        //     steps {
        //        echo "${CC}"
        //        echo "${params.Greeting} World!"
        //         script {
        //             def repo = checkout scm
        //             echo "${repo}"
        //             echo repo.GIT_BRANCH.take(20).replaceAll('/', '_')
        //         }
        //     }
        // }
    }
}
