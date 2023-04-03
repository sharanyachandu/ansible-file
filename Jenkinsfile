pipeline {
    agent { label 'ws' }
    stages {
        stage('Performing Ansible Dry Run') {
            steps {
                sh "ansible-playbook robot-dryrun.yaml -e COMPONENT=mongodb -e ansible_user=centos -e ansible_password=DevOps321 -e ENV=qa"
            }
        }
    }
}