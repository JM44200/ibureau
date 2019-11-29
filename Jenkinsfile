pipeline {
    agent any 
    
    tools {
            maven 'M3'
    }
    
    stages {
        stage('Build') { 
            steps {
                echo 'Etape Hello, Build Maven'
                bat 'mvn clean compile'
            }
        }
        stage('Test') { 
            steps {
                echo 'Etape Hello, Test Maven'
                bat 'mvn clean test'
            }
        }
        stage('Packaging') { 
            steps {
                echo 'Etape Hello, Panckaging Maven'
                bat 'mvn clean package'
            }
        }
        stage('Deploy') { 
            steps {
                // 
                echo 'Etape Deploy'
            }
        }
    }
}
