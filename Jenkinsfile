@Library("shared-lib") _
pipeline {
    agent { label 'docker' }
    stages {
        stage('Build') {
            steps {
                script {
                   main.callTestScript()
                }
            }
        }
    }
}
