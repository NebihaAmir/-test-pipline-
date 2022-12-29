pipeline {
    agent any

    stages {
        stage('Starting') {
            steps {
                echo 'Building Project'
            }
        }
       
        stage('Connecting with GIT') {
            steps {
                 git changelog: false, url: 'https://github.com/pavansw/keeplearning.git'
            }
        }
       
        stage('CRun Python Code') {
            steps {
//                  sh 'python hello.py'
                sh -c 'echo "Hello, world!"'
            }
        }
        
    }
}
