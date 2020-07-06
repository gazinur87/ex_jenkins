pipeline {
     agent {
        kubernetes {
            label 'PodLabel2'
            defaultContainer 'busybox'
//             yaml """
// apiVersion: v1
// kind: Pod
// metadata:
//   labels:
//     job: build-service
// spec:
//   containers:
//   - name: busybox
//     image: busybox
//     command: ["cat"]
//     tty: true
// """
        }
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
        stage('call') {
            steps {
               container('busybox') {
                   hostname
                }
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
