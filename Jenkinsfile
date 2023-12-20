pipeline {
    agent {
        docker { image:'docker pull maven:3.8.8-eclipse-temurin-8-alpine'}
    }
    stages {
        stage ('verson info') {
            steps {
                git 'https://github.com/Tirumaleshnaidu/maven-web-application.git'
                sh 'mvn --version'
                sh 'mvn clean package'
            }
        }
    }
}
