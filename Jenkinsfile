pipeline {
    agent any
 
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Jitendraphirke/JenkinsJavaProject.git'
            }
        }
      stage('restore') {
            steps {
                bat 'mvn clean compile'
            }
        }
      stage('build') {
            steps {
                bat 'mvn clean compile'
            }
        }
      stage('test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
