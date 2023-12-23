 pipeline {
    agent any
    environment {
        SSH_CRED= credentials ('SSH_CRED')
    }
    stages {
        stage("Performing dry run") {
            steps {
                sh "env"
                sh "ansible-playbook -i inv-robot -e COMPONENT=frontend -e ansible_user=${SSH_CRED_USR} -e ansible_password=${SSH_CRED_PSW}"
            }
        }
        }
    }