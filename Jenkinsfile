pipeline {
  environment {
    registry = "pratush43/dock"
    registryCredential = 'dockerhub'
  }
  agent none
    stages {
        stage('Build') {
          agent {
    node{
    label 'micro'
    } 
  }
            steps {
              sh 'cd Core_HelloWorld'
                sh 'dotnet build'
            }
        }
        
    }
      
}
