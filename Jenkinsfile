def HELLO = "danielsgg";

pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                script {
                    echo "The Test Started"
                }
            }
        }
        stage('If-Else') {
            steps {
                catchError {
                    script {
                        //echo "I am ${HELLO}"
                        if (HELLO == "daniel") {
                            echo "I am Daniel"
                        } 
                        else if (HELLO == "danielsg") {
                            echo "I am not Daniel"
                        } else {
                            echo "Daniel not found"
                        }
                    }
                }
            }
        }
        stage('Ended') {
            steps {
                script {
                    sh "echo The Test Ended"
                }
            }
        }
    }
}
