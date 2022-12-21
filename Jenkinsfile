pipeline{
    agent{
        label{
            lable'22Q2'
            customWorkspace'/mnt/visha2'
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
                sh "echo 'hey'>>/var/www/html/index.html"
                sh "chmod 777 /var/www/html/index.html"
            }
        }
    }
}
  
