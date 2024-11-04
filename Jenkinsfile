pipeline {
    agent any
    stages {
        stage('SCM') {
            steps {
                // Git checkout
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh './mvn clean install'
            }
        }
    }
}
