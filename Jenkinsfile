pipeline{
    agent{
        label{
            label'built-in'
            customWorkspace'/mnt/Sayli/'
        }
    }
    stages{
        stage('stage seq'){
            steps{
                sh " rm -rf *"
                sh "mkdir A"
            }
        }
        stage('parallel'){
            parallel{
                stage('stage-1'){
                    steps{
                        sh "mkdir B"
                    
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
                
                sh "touch 11 12 13 14"
                
            }
        }
    
    }
}
