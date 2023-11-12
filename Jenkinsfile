pipeline {
    agent any
    environment {
        PATH = "/opt/homebrew/bin:$PATH"
    }
   stages {
        stage('Deploy with Ansible') {
            steps {
                script {
                    ansiblePlaybook installation: 'Ansible', playbook: 'playbook.yaml', vaultTmpPath: ''
                }
            }
        }
    }
}
