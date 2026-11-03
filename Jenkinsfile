pipeline {
    agent any

    tools {
        jdk 'JDK21'
        maven 'Maven3.9.16'
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
