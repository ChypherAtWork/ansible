@Library("shared-lib") _
pipeline {
    agent any
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
