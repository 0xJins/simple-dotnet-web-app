pipeline {
  agent any
  environment {
      DOTNET_SYSTEM_GLOBALIZATION_INVARIANT = 1
  }
  stages {
    stage('Build') {
      steps {
        withDotNet(sdk: '.NET 6') {
      sh '''
            dotnet restore
            dotnet build
          '''
        }
      }
    }    
  }
}