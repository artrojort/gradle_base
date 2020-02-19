pipeline {
    agent {label 'swarm'}
    stages {
        stage('Test') {
            steps {
		sh 'chmod +x ./gradlew'
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
