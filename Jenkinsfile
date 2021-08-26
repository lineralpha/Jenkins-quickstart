node {
    docker.image('node:14-alpine').inside {
        stage('Test') {
            sh 'node --version'
            sh 'echo "Done!"'
        }
    }
}

// node {
//     checkout scm
//     try {
//         stage('Build') {
//             docker.image('node:14-alpine').inside {
//                 sh 'echo "Hello World!"'
//                 sh 'npm --version'
//             }            
//         }

//         stage('Test') {
//             sh 'echo "Fail!"; exit 1'
//         }

//         echo 'This will run only if successful'
//     }
//     catch (e) {
//         echo 'This will run only if failed'

//         // Since we're catching the exception in order to report on it,
//         // we need to rethrow it, to ensure that the build is marked as failed.
//         throw e
//     }
//     finally {
//         def currentResult = currentBuild.result ?: 'SUCCESS'
//         if (currentResult == 'UNSTABLE') {
//             echo 'This will run only if the run was marked as unstable'
//         }

//         def prevResult = currentBuild.previousBuild?.result
//         if (prevResult != null && prevResult != currentResult) {
//             echo 'This will run only if the state of the pipeline has changed'
//             echo 'For example, if the pipeline was previously failing but is now successful'
//         }

//         echo 'This will always run'
//     }
// }