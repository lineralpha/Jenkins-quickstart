pipeline {
    agent { docker { image 'maven:3.8.2-openjdk-8' }}
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
