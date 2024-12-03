pipeline{
    agent any
    stages {
        stage('Clean-up'){
            steps{
                deleteDir()
            }
        }
        
        stage('Clone Code'){
            steps{
                sh "git clone https://github.com/devopsPRO27/tictactoe.git"
            }
        }
        
        stage('Scan files'){
            steps{
                dir('tictactoe') {
                    sh "ls -lh"
                    sh "pwd"
                }
            }
        }
        
        stage('Test'){
            steps{
                sh "ls -lh"
                // mail bcc: '', body: 'This is a Jenkins test', cc: '', from: '', replyTo: '', subject: 'Test Jenkins Email Feature', to: 'barabudy@gmail.com'
            }
        }
        
    }
}