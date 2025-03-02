pipeline {
    agent any
    tools {
        nodejs 'NodeJS'  // This assumes you have a NodeJS tool configured in Jenkins
    }
    stages {
        stage('Github') {
            steps {
                git branch: 'main', credentialsId: 'Victorwasonga-cicd', url: 'https://github.com/Victorwasonga/Simple_NodeJS_App.git'
            }
        }
        stage('Unit Test') {
            steps {
                sh 'npm install'
                sh 'npm test'
            }
        }
    }
}
