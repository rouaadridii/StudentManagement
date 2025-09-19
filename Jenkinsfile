pipeline {
    agent any
    tools {
        maven 'maven'
        jdk 'jdk17'
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/rouaadridii/StudentManagement.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

