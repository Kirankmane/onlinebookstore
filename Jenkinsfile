pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
                git 'https://github.com/Kirankmane/onlinebookstore.git'
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

        stage ("Deploy to Tomcat") {
            steps { 
                sh 'sudo cp  -R /var/lib/jenkins/workspace/Online-book-store/target/onlinebookstore.war /opt/tomcat/apache-tomcat-9.0.68/webapps/'
            }
        }
    }
}

        
