pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
              sh "mvn clean -f sample-java-programs"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test -f sample-java-programs"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package -f sample-java-programs"
            }
        }
    }
}
