@Library('my-global-shared-library') _


pipeline {
    agent any
    
    stages {

        stage('SCM') {
            steps{
                checkout scm
            } 
        }
    }
    stage('SonarQube Analysis') {
        def scannerHome = tool 'SonarScanner';
        withSonarQubeEnv() {
        sh "${scannerHome}/bin/sonar-scanner"
            }
        }










        stage('Simple Hello') {
            steps {
                script {
                    helloWorld("Michael","Monday","you are a gem")
                }
            }
        }
        stage('Get Date') {
            steps {
                script {
                    // Call the method from the shared library
                    def currentDate = GetDate.getCurrentDateTime()
                    echo "Current date and time: ${currentDate}"
                }
            }
    }
}
}
   
