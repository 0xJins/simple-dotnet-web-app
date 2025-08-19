pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                withDotNet(sdk: '.NET8') {
                        sh 'dotnet restore' 
                        sh 'dotnet build --no-restore' 
                }
            }
        }
    }
}