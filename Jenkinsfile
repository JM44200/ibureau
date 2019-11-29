pipeline {
    agent any 
    
    tools {
            maven 'M3'
    }
    
    stages {
        stage('Build') { 
            steps {
                echo 'Etape Helloi, Build Maven'
                bat 'mvn clean compile'
            }
        }
        stage('Test') { 
            steps {
                // 
                echo 'Etape Test'
            }
        }
        stage('Packaging') { 
            steps {
                // 
                echo 'Etape Packaging'
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
