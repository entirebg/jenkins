pipeline {
    agent any

    stages {
        stage('Debug') {
            steps {
                script {
                    ansiblePlaybook(
                        become: true,
                        installation: 'Ansible',
                        playbook: 'playbook.yaml',
                        vaultTmpPath: ''
                    )
                }
            }
        }
        // ...
    }
}
