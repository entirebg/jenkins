pipeline {
    agent any

    environment {
        PATH = "/opt/homebrew/bin:$PATH"
    }

    stages {
        stage('Deploy with Ansible') {
            steps {
                script {
                    sh "/opt/homebrew/bin/ansible-playbook --version"
                }
            }
        }
    }
}

