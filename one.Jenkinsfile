pipeline{
    agent any
    environment { 
        SSH_CRED = credentials ('SSH_CRED')
    }
    stages {
        stage ('performing a dry run'){
            steps{
                sh "env"
                sh "ansible-playbook robot-dryrun.yml -e COMPONENT=mongogdb -e ansbile_usename=${SSH_CRED_USR} ansobile_password=${SSH_CRED_PSW}"
            }
        }
    }
}