pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/OmarYoness/omaryonessdemo1.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    sh 'javac src/main/java/Main.java'
                }
            }
        }

        stage('Run') {
            steps {
                script {
                    sh 'java -cp src/main/java Main'
                }
            }
        }
    }
}
