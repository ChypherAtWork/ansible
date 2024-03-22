@Library("shared-lib") _ 
pipeline {
    agent { label 'spot-ai' }
    options { timestamps() }
    environment {
        GIT_CRED        = credentials('Github-Read')
        PYPI            = credentials('pypi-admin-creds')
        PYPI_REPO       = 'https://pypi.qritive.com/simple/'
        SECRET_FILE     = credentials('version-file')
    }
    stages {
        stage('Build an Updated Tag') {
            steps {
                script {
                    main()
                }
            }
        }
    }
}
