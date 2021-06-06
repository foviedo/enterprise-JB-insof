pipeline {
  agent any
    stages {
        stage('Build') {
            steps {
                sh "git pull origin main"
   				sh './gradlew clean build'
                sh "./gradlew bootRun"
            }
        }
        stage('Test') {
            steps {
                sh "gradle test"
            }
        }
        stage('Validate') {
            steps {
                echo 'Validate....'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
		}
  }
}