@Library("shared-lib") _
pipeline {
    agent docker
    stages {
        stage('Build') {
            steps {
                script {
                    def groovyScript = load 'test.groovy'
                    groovyScript.call()
                }
            }
        }
    }
}
