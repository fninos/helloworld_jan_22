pipeline {
    agent any
    tools {
        stage('Build') {
            steps {
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Step'
                sleep 10
            }
        }
        stage('Docker') {
            steps {
                echo 'Image step'
            }
        }
    }
}
