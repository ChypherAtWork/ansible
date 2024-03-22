@Library("shared-lib") _
pipeline {
    agent { label 'docker' }
    stages {
        stage('Build') {
            steps {
                script {
                    def main = load ('src/main.groovy')
                    main()
                }
            }
        }
    }
}
