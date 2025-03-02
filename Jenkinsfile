pipeline {
    agent any
    stages{
        stage("Github"){
            steps{
                git branch: 'main', credentialsId: 'Victorwasonga-cicd', url: 'https://github.com/Victorwasonga/Simple_NodeJS_App.git'
            }
        }
    }




}
