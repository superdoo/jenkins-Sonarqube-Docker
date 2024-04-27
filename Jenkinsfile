@Library('my-global-shared-library') _

pipeline {
    agent any
    stages {
             
        stage('Say Hello') {
            steps {
                script {
                    // Call the function from the shared library
                    greetings.greet('Alice')
                }
            }
        }
    }
}
        
