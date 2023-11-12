pipeline {
    agent any

    stages {
         stage('Build') {
            steps {
                ansiblePlaybook installation: 'Ansible', playbook: 'playbook.yaml', vaultTmpPath: ''
                script {
                    sh "ansible-playbook playbook.yaml"
                }
            }
        }
        // ...
    }
}
