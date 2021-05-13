pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('build'){
            steps{
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline is for shopping-portal application... on Thu 13-May-2021 at 16:35:00 EDT'
        }
        
    }
    
}
