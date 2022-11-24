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
              dir('Core_HelloWorld')
                sh 'dotnet build'
            }
        }
        
    }
      
}
