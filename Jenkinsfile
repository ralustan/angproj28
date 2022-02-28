pipeline {
  agent { docker { image 'trion/ng-cli-karma:6.2.1' } }
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
            
        
    

