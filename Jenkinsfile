@Library('my-global-shared-library') _


pipeline {
    agent any
    
    stages {
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
                    // Load the DateUtils class
                    def dateUtils = load 'GetDate.groovy'
                    
                    // Call the getCurrentDateTime() method
                    def currentDate = DateUtils.getCurrentDateTime()
                    
                    // Print the current date and time
                    echo "Current date and time: ${currentDate}"
                }
            }
        }
    }
}
   
