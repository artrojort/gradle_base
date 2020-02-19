pipeline {
    agent {label 'swarm'}
    stages {
        stage('Test') {
            steps {
                sh 'sudo ./gradlew clean test --no-daemon' 
            }
	}
	stage('Build') {
	    steps {
		sh 'sudo ./gradlew build'
	    }
        }
    }
}
