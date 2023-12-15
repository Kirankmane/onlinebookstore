pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
                sh git 'https://github.com/Kirankmane/onlinebookstore.git'
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
    }
}

        
