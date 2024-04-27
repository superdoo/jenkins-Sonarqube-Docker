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
                    def GetDate = DateUtils() 
                   // def currentDate = dateUtils.getCurrentDateTime() // Call the method
                    // echo "Current date and time: ${currentDate}"
            
                }
            }
        }
    }
}
   
