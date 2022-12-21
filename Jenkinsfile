pipeline{
    agent{
        label{
            label'master'
            customWorkspace'/mnt/vishal'
        }
    }
    stages{
        stage('install apache server'){
            steps{
                sh "yum install httpd -y"
            }
        }
        stage('service start'){
            steps{
                sh "service httpd start"
                sh "rm -rf /var/www/html/index.html"
                sh "echo 'good night'>>/var/www/html/index.html"
                sh "chmod 777 /var/www/html/index.html"
            }
        }
    }
}
  
