pipeline {
    agent any

    stages {
        stage("build") {
            steps {
                sh """
                    docker build -t java-app .
                """
            }
        }
        stage("run") {
            steps {
                sh """
                    docker run --rm java-app
                """
            }
        }
    }
}
