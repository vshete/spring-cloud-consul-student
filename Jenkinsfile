pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            	echo 'now runnign mvn clean install ....'
                sh 'mvn clean install'
            }
        }
        stage ('declare completion') {
        	steps {
        		echo 'build completed successfully.'
        	}
        }
    }
}
