pipeline {
  agent any
    stages {
        stage('Build') {
            steps {
                sh "npm install"
                sh "ng build"
            }
        }
        stage('Test') {
          steps{
            
              sh 'ng test --progress=false --watch false'
          }
        }
        
    }
}
            
        
    

