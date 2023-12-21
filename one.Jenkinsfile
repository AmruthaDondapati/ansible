pipeline{
    agent any
    environment { 
        SSH_CRED = credentials ('SSH_CRED')
    }
    stages {
        stage ('performing a dry run'){
            steps{
                sh 'env'
                sh 'ansible-playbook robot'
            }
        }
    }
}