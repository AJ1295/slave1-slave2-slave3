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
                sh "mkdir AC"
            }
        }
        stage('parallel'){
            parallel{
                stage('stage-1'){
                    steps{
                        sh "mkdir BD"
                    
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
                
                sh "touch 1@1 122 123 124"
                
            }
        }
    
    }
}
