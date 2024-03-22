@Library("shared-lib") import main
pipeline {
    agent { label 'docker' }
    stages {
        stage('Build') {
            steps {
                script {
                    test()
                }
            }
        }
    }
}
