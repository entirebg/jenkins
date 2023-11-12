pipeline {
    agent any

    stages {
        stage('Debug') {
            steps {
                script {
                    sh "id"
                    sh "ansible-playbook"
                }
            }
        }
        // ...
    }
}
