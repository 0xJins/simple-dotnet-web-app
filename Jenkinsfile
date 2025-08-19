pipeline {
    agent any
    stages {
        stage('Build') { 
            withDotNet(sdk: '.NET8') {
                steps {
                    sh 'dotnet restore' 
                    sh 'dotnet build --no-restore' 
                }
            }
        }
    }
}