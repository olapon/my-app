pipeline {
    agent any 
    stages {
        stage('--Clean Repo--') { 
            steps {
                bat "mvn clean"
            }
        }
        stage('--Test mvn--') { 
            steps {
                bat "mvn test"
            }
        }
        stage('--Deploy mvn--') { 
            steps {
                bat "mvn package"
            }
        }
        stage('--Status--') { 
            steps {
                bat "git"
            }
        }
    }
}
