pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
git 'https://github.com/Prathimajogannagari/OlxUsersMicroservice.git'
            }
        }

    
        stage('compile') {
            steps {
                bat 'mvn clean compile'
            }
        }
        stage('Run') {
            steps {
              bat 'mvn package'
            }
        }
             stage('Test Report using jacoco') {
            steps {
                echo 'jacoco'
            }
        }
          stage('Building Docker Image') {
            steps {
                echo 'Building Docker Image'
            }
        }
    }
}
