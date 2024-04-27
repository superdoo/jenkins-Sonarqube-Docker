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
        stage('Geto Dateo') {
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
   
