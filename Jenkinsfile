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
        stage('Packaging') { 
            steps {
                echo 'Hello, Packaging Maven'
                bat 'mvn clean package'
            }
        }
        stage('Deploy') { 
            steps {
               echo 'Hello, Deploy'
               bat ' copy "target\\ebureau.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps" '
            }
        }
    }
}ebureau.war
