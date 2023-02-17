pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o error'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './pes2ug20cs026.exe'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
