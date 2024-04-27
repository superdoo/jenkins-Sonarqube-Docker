@Library('my-global-shared-library') _

pipeline {
    agent any
    stages {
             
        stage('greetings') {
            steps {
                script {
                    // Call the function from the shared library
                    my-global-shared-library.greet('Alice')
                }
            }
        }
    }
}
        
