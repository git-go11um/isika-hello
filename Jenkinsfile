pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo '-----Collecting to Github-------'
                git branch: 'main', url: 'https://github.com/git-go11um/isika-hello'
            }
        }
        stage('Compile') {
            steps {
                echo '-----Compiling Code-------'
                bat 'javac *.java'
            }
        }
        stage('Run') {
            steps {
                echo '-----Running Application-------'
                bat 'java Hello'
            }
        }
    }
}