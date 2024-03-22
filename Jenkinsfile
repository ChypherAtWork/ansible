@Library("shared-lib") _
pipeline {
    agent { label 'docker' }
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
