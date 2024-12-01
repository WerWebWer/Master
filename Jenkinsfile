pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    try {
                        sh './gradlew build --no-daemon' //run a gradle task
                    } finally {
                        echo 'Build done'
                    }
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
