pipeline {
	tools{
	jdk 'JAVA_HOME'
	maven 'M2_HOME'
	}
    agent {label 'WinLabelsNode'}

    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/satyachoudhury101/Repo1.git'
            }
        }
		stage('compile') {
            steps {
                bat 'mvn compile'
            }
        }
		stage('test') {
            steps {
                bat 'mvn test'
            }
        }
		stage('package') {
            steps {
                bat 'mvn package'
            }
		}
	}
}
	
        
