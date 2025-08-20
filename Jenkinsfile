pipeline {
    agent any

    tools {
        maven 'M3'  // el nombre que pusiste en Global Tool Configuration
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Maylie-cloud/calculadora.git'
            }
        }
        stage('Validate Syntax') {
            steps {
                bat 'mvn clean validate'
            }
        }
    }
}

