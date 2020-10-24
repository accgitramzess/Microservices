pipeline {

    agent any

    stages {
        stage('Start') {
            stages {
                stage('Init') {
                    steps {
                        sh './gradlew clean --no-daemon'
                    }
                }

                stage('Compile') {
                    steps {
                        sh './gradlew compileJava compileTestJava --no-daemon'
                    }
                }

                stage('Check') {
                    steps {
                        sh './gradlew check --no-daemon'
                    }
                }

                stage('Unit') {
                    steps {
                        sh './gradlew test'
                    }
                }
            }
        }
    }
}