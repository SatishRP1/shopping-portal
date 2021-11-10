pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
  tools{
       Nodejs'Maven 3.6.3' 
    }    

    stages{
        stage('build'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
                
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
                
            }
        }
        stage('Package'){
            steps{
                echo 'this is the packagejob'
                sh 'npm run package'
                
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
