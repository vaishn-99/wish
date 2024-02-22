pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App!'
            }
        }
        stage('Test') {
            steps {
                echo 'Test App!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'Pipeline has run successfully!', subject: 'Pipeline Status', to: 'dsrhemanth@gmail.com'
        }
    }
}
