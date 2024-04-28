@Library('my-global-shared-library') _


pipeline {
    agent any

      def scannerHome = tool 'SonarScanner'
    
    stages {

           
             




        stage('SCM') {
            steps{
                checkout scm
            } 
        }
    
            stage('SonarQube Analysis') {
            steps {
                script {
                    def sonarQubeUtils = new SonarQubeUtils() // Instantiate the SonarQubeUtils class
                    def projectName = 'Onix-website-scan'
                    def projectKey = 'Onix-website-scan'
                    def scannerHome = '/path/to/sonar-scanner'
                    sonarQubeUtils.callSonarQubeScanner(projectName, projectKey)
                }
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

   
