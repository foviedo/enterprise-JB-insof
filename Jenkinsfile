pipeline {
  agent any
    stages {
        stage('Build') {
            steps {
                sh "git pull origin main"
   				sh 'bash ./gradlew clean build'
                sh "bash ./gradlew bootRun"
            }
        }
        stage('Test') {
            steps {
                echo 'Testeing...'
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