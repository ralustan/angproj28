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
            withEnv(["CHROME_BIN=/usr/bin/chromium-browser"]) {
              sh 'ng test --progress=false --watch false'
        }
        junit '**/test-results.xml'
    }
            
        
    }
}
