pipeline {
    agent any
  
    stages  {
        stage('check the status of tomcat9') {
            steps {
                sh 'systemctl status tomcat9'
            }
        }
        stage('copy index.html to your tomcat9 home directory') {
            steps {
                sh 'cp index.html /var/lib/tomcat9/webapps/abcd'
            }
        }
        stage('final stage') {
            steps {
                sh 'echo "job completed"'
            }
        }
 }
}
