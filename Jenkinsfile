pipeline {
    agent any
    environment {
                 JAVA_HOME="C:\\Program Files\\Java\\jdk-14.0.2"
    }
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                bat "git clone https://github.com/RAGAVIKRISHNA/Planit-Automation-Assessment.git"
                bat "C:\\Users\\maven\\apache-maven-3.8.1\\bin\\mvn clean verify"
                bat "rmdir /s/q Planit-Automation-Assessment" 
}
            

            post {
                // If Maven was able to run the tests, even if some of the test
                // failed, record the test results and archive the jar file.
                success {
                    junit '**/target/surefire-reports/TEST-*.xml'
                    archiveArtifacts 'target/*.jar'
                }
            }
        }
    }
}
