pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG21CS403-1.cpp -o temp'
                 build job: 'PES1UG21CS403-1', wait: false
                 echo 'Build by CS403 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG21CS403-1.cpp'
                echo 'Test by CS403 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS403 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
