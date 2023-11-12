pipeline {
    agent any
    environment {
        PATH = "/opt/homebrew/bin:$PATH"
    }
   stages {
        stage('Deploy with Ansible') {
            steps {
                script {
                    def result = sh(script: '/opt/homebrew/bin/ansible-playbook playbook.yaml', returnStatus: true)
                    echo "Exit Code: ${result}"
                }
            }
        }
    }
}
