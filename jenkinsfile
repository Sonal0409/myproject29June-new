pipeline{
    
    tools{
        maven 'mymaven'
    }
    
    agent any
    
    stages{
        stage('clone repo'){
            steps{
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        
        stage('compile code'){
            steps{
               sh 'mvn compile'
            }
        }
        
         stage('code review'){
            steps{
               sh 'mvn pmd:pmd'
            }
        }
    }
}
