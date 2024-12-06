pipeline {
    agent {
        any
        // label: cloud - native
        // docker: alpine
    }
    stages{
        stage("Cloning") {
            steps{
                echo "=====Cloning git repo====="
                sh "git clone git.repo"
            }
            post {
                always {
                    echo "==always=="
                }
                success {
                    echo "==in case of success=="
                }
                failure {
                    echo "==in case of failure=="
                }
            }
        }
    }
    post { // post for the entire stages part
        success {
            echo "==Pipeline-success=="
        }
        failure {
            echo "==Pipeline-failure=="
        }
    }
}