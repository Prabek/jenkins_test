pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
            }
        }
        
         stage('Test') {
            steps {
                echo 'Hello World'
            }
        }
        
         stage('Deploy') {
            steps {
                echo 'Hello World'
            }
        }
        
    }
    
     post {
        always {
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
}
