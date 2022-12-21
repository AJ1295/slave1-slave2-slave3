[200~pipeline{
    agent{
        label{
            label'built-in'
            customWorkspace'/mnt/Shital/'
        }
    }
    stages{
        stage('stage seq'){
            steps{
                sh "mkdir a"
            }
        }
        stage('parallel'){
            parallel{
                stage('stage-1'){
                    steps{
                        sh "mkdir b"
                    
                    }
                }
                stage('stage-2'){
                    steps{
                        sh "yum install tree -y"
                    }
                }
            }
        }
        stage('seq 2'){
            steps{
                
                sh "touch 1 2 3 4"
                
            }
        }
    
    }
}
