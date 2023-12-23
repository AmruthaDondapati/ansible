 pipeline {
    agent any
    environment {
        SSH_CRED= credentials ('SSH_CRED')
    }
    stages {
        stage("Performing dry run") {
            steps {
                sh "env"
            }
        }
        }
    }
}