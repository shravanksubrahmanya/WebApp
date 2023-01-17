pipeline {
    agent any

    stages {
        stage('x') {
            steps {
                echo 'Hello x'
            }
        }
        stage('y') {
            steps {
                echo 'Hello y'
            }
        }
        stage('z') {
            steps {
                echo 'Hello z'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'successful build', subject: 'congrats', to: 'anotheruserdead@gmail.com'
        }
    }
}
