pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o pes2ug20cs026.exe working.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './pes2ug20cs026.exe'
            }
            
        stage('Deploy'){
			steps{
				echo 'Deployed Successfully'
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
