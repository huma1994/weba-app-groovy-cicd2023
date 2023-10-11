pipeline{
    agent any
    environment{
        staging_server="192.168.1.160"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh scp -r ${WORKSPACE}/* root@${staging_server}:/usr/share/nginx/html/star}              
            }
        }
    }
}
