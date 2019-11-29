pipeline {
    agent any 
    
    tools {
            maven 'M3'
    }
    
    stages {
        stage('Build') { 
            steps {
                echo 'Hello, Build Maven'
                bat 'mvn clean compile'
            }
        }
        stage('Test') { 
            steps {
                echo 'Hello, Test Maven'
                bat 'mvn clean test'
            }  
        }
        stage('Sonar') { 
            steps {
                echo 'Hello, Test Sonar'
                bat 'mvn clean test'
            }
        }
        stage('Packaging') { 
            steps {
                echo 'Hello, Packaging Maven'
                bat 'mvn clean package'
            }
        }
        stage('Deploy') { 
            steps {
               echo 'Hello, Deploy'
               bat ' mvn sonar:sonar -Dsonar.host.url=http://localhost:9000 -Dsonar.login=7853facbc9ca77bca43cfe244cb567a56d587501 '
            }
        }
    }
}
