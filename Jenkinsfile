pipeline {
 agent "dockerL1"
 
          //  defaultContainer 'busybox'
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
    

    stages {
        stage('call') {
            steps {
   //            container('busybox') {
                   sh "hostname"
 //               }
            }
        }

    
    }
}
