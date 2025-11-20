pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'
    }
    stages {
        stage('clean') {
            steps {
                echo "cleaning"
                bat "mvn clean"
            }
        }
        stage('install') {
            steps {
                echo "installing and building"
                bat "mvn install"
            }
        }
        stage('test') {
            steps {
                echo " testing..."
                bat "mvn test"
            }
        }
        stage('package') {
            steps {
                echo "packaging"
                bat "mvn package"
            }
        }
    }
}
