pipeline {
  agent any
    stages {
        stage('Build') {
            steps {
                sh "git pull origin main"
                echo 'Building...'
                echo 'Ejecutando el jar...'
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