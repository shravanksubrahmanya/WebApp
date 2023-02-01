pipeline {
    agent any

    stages {
        stage('integrate') {
            steps {
                echo 'Hello x'
            }
        }
        stage('build') {
            steps {
                echo 'Hello y'
            }
        }
        stage('test') {
            steps {
                echo 'Hello z'
            }
        }
        stage('deploy') {
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
