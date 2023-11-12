pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                ansiblePlaybook installation: 'Ansible', playbook: 'playbook.yaml', vaultTmpPath: ''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
