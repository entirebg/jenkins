pipeline {
    agent any
    environment {
        PATH = "/opt/homebrew/bin:$PATH"
    }
   stages {
        stage('Deploy with Ansible') {
            steps {
                script {
                    sh 'env'
                    sh '/opt/homebrew/bin/ansible-playbook playbook.yaml'
                }
            }
        }
    }
}
