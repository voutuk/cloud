pipeline {
    agent any

    stages {
        stage('docker-build-front') {
            steps {
                script {
                    // Use 'sh' step to execute shell commands
                    sh 'docker build /var/lib/jenkins/workspace/Diplom/FrontEnd/my-app/ --tag=front'
                }
            }
        }
        stage('docker-run-front') {
            steps {
                script {
                    // Use 'sh' step to execute shell commands
                    sh 'docker run -d -p 80:80 front'
                }
            }
        }
    }
}
