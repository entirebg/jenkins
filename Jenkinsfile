pipeline {
    agent any

    stages {
        stage('Debug') {
            steps {
                script {
                    sh 'env'
                    sh '/opt/homebrew/bin/ansible-playbook playbook.yaml'
                }
            }
        }
        // ...
    }
}
