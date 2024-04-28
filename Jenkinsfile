@Library('my-global-shared-library') _


pipeline {
    agent any
    
    stages {

        stage('SCM') {
                 checkout scm
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
   
