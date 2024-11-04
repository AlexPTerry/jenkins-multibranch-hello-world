pipeline {
    agent any

    tools {
        maven "M3"
    }

    stages {
        stage('SCM') {
            steps {
                // Git checkout
                checkout scm
            }
        }
        stage('Compile') {
            steps {
                sh "mvn clean compile"
            }
        }
    }
}
