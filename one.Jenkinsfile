pipeline{
    agent any
    environment { 
        SSH_CRED = credentials ('SSH_CRED')
    }
    stages {
        stage ('performing a dry run'){
            steps{
                sh "env"
                sh "ansible-playbook robot-dryrun.yml -e COMPONENT=mongodb -e ansible_usename=centos -e ansible_password=DevOps321"
            }
        }
    }
}