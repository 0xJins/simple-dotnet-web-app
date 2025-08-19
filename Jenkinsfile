pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                withDotNet(sdk: '.NET 8') {
                        sh 'dotnet restore' 
                        sh 'dotnet build --no-restore' 
                }
            }
        }
    }
}