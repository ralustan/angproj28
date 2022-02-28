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
            
              sh 'ng test --progress=false --watch false'
        }
        junit '**/test-results.xml'
    }
            
        
    }
}
