pipeline {
    agent any
    tools {
        nodeJS 'NodeJS' // Corrected to nodeJS
    }
    stages {
        stage("Github") {
            steps {
                git branch: 'main', credentialsId: 'Victorwasonga-cicd', url: 'https://github.com/Victorwasonga/Simple_NodeJS_App.git'
            }
        }
        stage("unit test") {
            steps {
                sh 'npm test'
                sh 'npm install'
            }
        }
    }
}
