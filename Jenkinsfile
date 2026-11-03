pipeline {
    agent any

    tools {
        jdk 'java'
        maven 'maven'
    }

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Run') {
            steps {
                bat 'java -cp target/classes Hello'
            }
        }
    }
}
