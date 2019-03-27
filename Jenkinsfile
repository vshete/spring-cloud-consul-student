pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            	echo 'now runnign mvn clean install ....'
                sh 'mvn clean install'
            }
        }
        stage ('Unit Tests') {
        	steps {
        		echo 'Running Unit tests'
        		sh 'mvn test'
        	}
        }
        stage ('Deploy') {
        	steps {
        		echo 'Starting the application'
        		sh 'mvn spring-boot:run'
        	}
        }
    }
}
