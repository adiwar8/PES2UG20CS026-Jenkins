
pipeline {
 agent any
	 stages {
		 stage('Build') {
		 steps {
			 sh 'g++ -o PES2UG20CS026-1 ./working.cpp'
			 echo 'Build stage has been completed successfully'
		 }
	 	}
		 stage('Test') {
			 steps {
			 ph './PES2UG20CS026-1'
			 echo 'Testing stage has been completed successfully'
			 }
		 }
		 stage('Deploy') {
			 steps {
			 echo 'Deploying stage has been completed successfuly'
			 }
		 }
	}
	post {
		failure {
		 	echo 'Pipeline failed'
		 }
	 }
}
