@Library('my-global-shared-library') _


pipeline {
    agent any
    
    stages {
        stage('Simple Hello') {
            steps {
                script {
                    helloWorld("Michael","Moonday","you are a gem")
                }
            }
        }

       stage('Getting The Date') {
            steps { 
                script {
                    currentDate()
                }
            }
        }  
    }
}
   
