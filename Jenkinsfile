pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
                sh git url
            }
        }

        stage ("Build Stage") {
            steps {
                sh 'mvn clean package'
                echo "build stage will be susscess"
            }
        }

        stage ("test") {
            steps {
                echo "test stage will be success"
            }
        }

        
