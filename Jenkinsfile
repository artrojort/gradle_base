pipeline {
    agent {label 'swarm'}
    stages {
        stage('Test') {
            steps {
                sh './gradlew clean test --no-daemon' 
            }
	}
	stage('Build') {
	    steps {
		sh './gradlew build'
	    }
        }
    }
}
