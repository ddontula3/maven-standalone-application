pipeline {
    agent any 
    stages {
        stage(' clean') { 
            steps {
               
                bat "mvn clean -f maven-standalone-application"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test -f maven-standalone-application"
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package -f maven-standalone-application"
            }
        }
    }
}
