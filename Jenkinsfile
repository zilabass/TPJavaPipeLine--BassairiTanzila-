pipeline {
    agent any
    
    stages {
        stage('Compile') {
            steps {
                echo 'Compiling Java program...'
                sh 'javac HelloWorld.java'
            }
        }
        
        stage('Run') {
            steps {
                echo 'Running Java program...'
                sh 'java HelloWorld'
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
