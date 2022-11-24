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
              dir("Core_HelloWorld"){
              sh 'cd Core_HelloWorld'
              sh 'pwd'
              sh 'ls -lrt'
              
                sh 'dotnet build'
            }
            }
        }
        
    }
      
}
