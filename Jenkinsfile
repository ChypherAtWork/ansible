@Library("shared-lib") _
pipeline {
    agent docker
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
