pipeline{
    agent{
        label{
            label'built-in'
            customWorkspace'/mnt/Shital/'
        }
    }
    stages{
        stage('stage seq'){
            steps{
                sh " rm -rf *"
                sh "mkdir AB"
            }
        }
        stage('parallel'){
            parallel{
                stage('stage-1'){
                    steps{
                        sh "mkdir BA"
                    
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
                
                sh "touch 111 112 113 114"
                
            }
        }
    
    }
}
