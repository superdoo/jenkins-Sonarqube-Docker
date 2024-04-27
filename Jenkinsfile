@Library('my-global-shared-library') _


pipeline {
    agent any
    
    stages {
        stage('Example') {
            steps {
                script {
                    // Call the function from the shared library
                    def message = MySharedLibrary.greetings()
                    echo message
                }
            }
        }
    }
}
   
